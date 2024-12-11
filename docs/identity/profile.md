!!! Warning "" 
	 :warning: <strong>This documentation site has been deprecated and will no longer be updated as of 11/11/24. Foundry applications are now part of the [Crucible Framework](https://cmu-sei.github.io/crucible/). The Identity applicaiton is no longer supported in the Crucible Framework.</strong>

# Profile

## Edit your Profile

Click **Profile**, then **Edit** to add information (**Name**, **Bio/status**, **Organization**, **Unit**) that helps to define who you are.

You can also add images for **Service Logo**, **Avatar**, and **Unit Logo**. Click **Change**, then **Choose File**. Add some descriptive tags to help others find the image file and click **Upload**.

## Credentials

Click **Credentials** to change your email address, password, and merge accounts.

To change your email address, enter your new email address and a *new* code. Click **Send Verification Code** to send the new code to the new email address. Any domain restrictions imposed by the Identity administrator apply here.

To change your password, enter your **current** password, **new password**, and your new password **again**. Then click **Submit**.

You can merge two accounts. This is useful if you received an updated certificate that is different from your previous certificate and logged in with it.

1. Log into Identity with the account you wish to *discard*.
2. Click **Get Merge Code**. Keep the merge code handy.
3. Log out of Identity.
4. Log into Identity with the account you wish to *keep*.
5. Enter your merge code, then click **Submit Merge Code**.

## Configure 2FA

You'll need to be logged into Identity, and be sure to do this while you do have access to email.

1. On your Identity profile, click **Configure 2FA**.
2. Click **Generate** to generate a time-based One Time Password (TOTP) secret key.
3. Use this secret key with any TOTP-enabled authentication app, such as Duo Mobile or Google Authenticator, by scanning the barcode. If you don't have access to your device, copy down the secret key and later input it into the TOTP app on your device.

You only need to generate the TOTP key (QR Code) once and register it with your authenticator app.  If you generate it again, it will replace the previous one and making it invalid. After registering the TOTP key (QR Code) with your authenticator app, the app should supply you a new code every 30 seconds.  Those codes are only valid one time within that 30-second window.

!!! note
    You can always continue to use the “registration code via email” option by clicking **Send me a code after logging in** – even if you have configured an authenticator app.