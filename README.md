# PasswordCryptographyProvider
Password Cryptography Provider implements OWASP recommendation password security - Salt and SHA512.

This implementation can be used in any java aplication to to encrypty password using SHA512 alogrithm with added security of Salt.

## Api 
1. ``` public String[] encrypt(final String password) ```

``` java 
/**
    * This method generates Salt and hashed Password
    *
    * @param password char array.
    * @return String array with [0] encoded salt [1] hashed password.
    */
```
2. ``` public String encrypt(final String password, String salt) ```

``` java 
 /**
    * This method re-generates hashed Password from raw-password and salt.
    * This will be used during authentication.
    *
    * @param password char array.
    * @param salt byte array.
    * @return byte array of hashed password.
    */
```
  

