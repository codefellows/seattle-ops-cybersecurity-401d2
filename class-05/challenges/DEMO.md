# Ops Challenge: File Encryption

## Demo Code

Here is the code that was demonstrated in class.

```powershell
# Encrypt a file
(Get-Item –Path "C:\Users\administrator\Desktop\I am not a cat.txt.txt").Encrypt()

# Decrypt a file
(Get-Item –Path "C:\Users\administrator\Desktop\I am not a cat.txt.txt").Decrypt()

# Generate an encrypted string from a plaintext string
"P@ssword1" | ConvertTo-SecureString -AsPlainText -Force | ConvertFrom-SecureString

# Generate a hash without specifying the algorithm
Get-FileHash "C:\Users\administrator\Desktop\I am not a cat.txt.txt" 

# Specify SHA256 algorithm explicitly
Get-FileHash "C:\Users\administrator\Desktop\I am not a cat.txt.txt" -Algorithm SHA256
```
