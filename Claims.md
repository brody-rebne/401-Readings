## Claims

- Claims are pieces of information assigned to an identity
- Claims are *not* authenticating
- Claims are name/value pairs which describe charicteristics of a subject
- Commonly used to allow specific sub-behaviors for users
- Identities may have any number of claims, even multiple of the same type
- Claims are declared via an inbuilt constructor `Claim claimName = new Claims("ClaimKey", "Claim Value")`
  - "ClaimKey" is the key to access the claim
  - Thus, this claim could be accessed in a razor file with the code `@User.Claims.First(x => x.Type == "ClaimKey").Value`
  - This will display the text "Claim Value"
- Can be added to an identity via inbuilt method `AddClaimAsync(user, claim)`
- More commonly, multiple can be added to a list, and added to an identity via inbuilt method `AddClaimsAsync(user, claimList)`
