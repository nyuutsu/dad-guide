# Phone Authentication Setup

# On your phone...

## Install an authenticator app on your phone

```admonish
This section contains screenshots. Each image shows how to do the step on iOS and on Android. The image on the left is iOS and the right is Android. 
```

### Find and open your phone's app store

Your phone has an "app store". On android, the app store app is named “play store”. On ios, it is named “app store”. Open your app store. 

![Phone](images/phone-1.png)

*Find and open your phone's app store.*

### Search "authenticator" + identify authenticator + install

In the search bar, search for “authenticator”. Select one from a major software publisher and install it.

```admonish
NDRN suggests using Google Authenticator. Microsoft Authenticator would work also.
```

![Phone](images/phone-3.png)

*Pick one of the search results*

In the search result, select an authenticator to be taken to its info page. Select "get" or "install" to download it and wait for it to install.

Once the authenticator installs, try running it. You should see something similar to mine. If you just installed your authenticator then it will have no entries yet. 

![Phone](images/example-auth.jpg)

*This is a screenshot of my authenticator - I use this for many services, so it already has some entries. I've blurred the names of those other services out.*

# On your computer...

## Attempt to log in to DAD

Attempt to log in to DAD. You should see a screen titled"Configure Authenticator App". The page should have a QR code (a square barcode thing) on it.

![Phone](images/phone-6.png)

*This screenshot is for illustration purposes. You will get your code from the DAD website. You will not get it from this image it is only an example.*

# On your phone...

## Use the authenticator to scan the QR code

In the authenticator app, tap the plus sign (+). Choose "Scan a QR code". This will launch a camera. Point it at the QR code shown in DAD. The authenticator camera should automatically take the information it needs, close the camera, and place you back at the authenticator's main screen with a new authenticator entry listed for DAD. Congratulations! You have set up your authenticator. Now all that's left is to use it. 

![Phone](images/qr-scan.jpg)

*Point camera at the QR code in DAD*


```admonish
The "scan a QR code" step only has to be done during setup. During a typical login after setup, you don't need (and won't be shown) another QR code. You'll open your authenticator, get your current six-digit code, and give that to DAD and you'll be "in". 
```

```admonish
What the QR code does is to tell your authenticator how to make the six-digit security code DAD is asking for. Once it knows how to do this, it doesn't need to be told how again. 
```

# On your computer, from your phone...

## Enter a code from your new DAD authenticator entry into DAD to confirm that setup worked

In your authenticator, there will be a six digit code. This code changes about every thirty seconds. Enter the current code (no spaces, just digits) into the "Verification Code" field in DAD and click the "Verify" button. You should now be logged in; congratulations! 

```admonish
Please don't delete the authenticator! You aren't going to need it especially often, but you do want it to be available. 
```