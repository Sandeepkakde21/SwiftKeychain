# SwiftKeychain
SwiftKeychain is a keychain wrapper class for storing and retriving data in to the keychain.

How to use SwiftKeychain.

1. Download zip folder which contain demo application.

2. Find file "KeychainService" and add it into your project.

3. Go to your view controller or view model and create shared instance of "KeychainService"
       let keychaine = KeychainService.sharedInstance
      
 4. To store data in keychain.     
        print(keychaine.saveSecureData(key: "key", value: "Test value"))
     
 5. To update data in keychain  
        print(keychaine.updateSecureData(key: "key", value: "updated value"))
        
 6. To get data from keychain      
        print(keychaine.loadSecureData(key: "key")!)
        
 7. To remove data from keychain.       
        print(keychaine.removeSecureData(key: "key"))
