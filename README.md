##AHCodesignVerifier
Simple class to check the code sign of an app bundle or executable. 

Currently there are only three methods

-
####To get the name of a certificate used to sign an item
```
+ (NSString*)certNameOfItemAtPath:(NSString*)path 
                            error:(NSError**)error;
```
-

####To test whether the codesign of an item is valid
```
+ (BOOL)codeSignOfItemAtPathIsValid:(NSString *)path
                              error:(NSError**)error;
```
-

####To compare two items.  
```
+ (BOOL)codesignOfItemAtPath:(NSString*)item1
          isSameAsItemAtPath:(NSString*)item2
                       error:(NSError**)error;
```
_* I use this in priviledged helper tools to check that the NSXPC message sender is valid_

-

See AHCodesignVerifier.h for more details

