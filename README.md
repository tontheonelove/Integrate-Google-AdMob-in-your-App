# Integrate-Google-AdMob-in-your-App



#Importent

private String TAG = SecondActivity.class.getSimpleName();

    InterstitialAd mInterstitialAd;
    
  
 # This is Show Full Screen
 
  mInterstitialAd = new InterstitialAd(this);
 
 
        // set the ad unit ID
        mInterstitialAd.setAdUnitId(getString(R.string.interstitial_full_screen));
        
 
        AdRequest adRequest = new AdRequest.Builder()
        
                .build();
 
        // Load ads into Interstitial Ads
        
        mInterstitialAd.loadAd(adRequest);
 
        mInterstitialAd.setAdListener(new AdListener() {
        
            public void onAdLoaded() {
            
                showInterstitial();
                
            }
            
        });
        
    }
 
    private void showInterstitial() {
    
        if (mInterstitialAd.isLoaded()) {
        
            mInterstitialAd.show();
        }
    }
 
}
    
    
    
    
    





<img src=android-integrating-admob-banner-interstitial.jpg/>
