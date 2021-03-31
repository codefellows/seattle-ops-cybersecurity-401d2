## Day 9 - Public Key Infrastructure (PKI)

  1. Notes
  2. Discussion
    1. [SSH.com What is Public Key Infrastructure (PKI)](https://www.ssh.com/pki/)
    2. [Prof Messer Security+ PKI Components](https://www.youtube.com/watch?v=3yuad7_bszE)
  3. Lecture
    1. Why use **Public key infrastructure (PKI)** (ref [SSH.com](https://www.ssh.com/pki/))
      1. Today's security professional, particularly at the entry level, needs to have a firm grasp of how and why PKI is used in various systems today.
      2. Secure websites
      1. Prevents man-in-the-middle attack
      2. "Lock" icon in browser - standard user experience
      3. Authenticating users and computers
      4. Email signing and encryption

    2. What is PKI?
      1. "Public Key Infrastructure (PKI) is a technology for authenticating users and devices in the digital world. The basic idea is to have one or more trusted parties digitally sign documents certifying that a particular cryptographic key belongs to a particular user or device. The key can then be used as an identity for the user in digital networks." (ref [SSH.com](https://www.ssh.com/pki/))
      2. Security functional purpose of PKI
        1. Identification
        2. Authentication
        3. Nonrepudiation
        4. Confidentiality
      3. Vocabulary
        1. CA = Certificate Authority
      4. Types
        1. Symmetric
          1. Advantage: Faster
          2. Examples: AES-128, AES-192, and AES-256
        2. Asymmetric
          1. Advantage: Nonrepudiation
            1. The sender and receiver vouch for who they are with their own private keys
          2. Examples: RSA, DSA, and PKCS
      5. Diagram: CA role in client-server PKI

![](RackMultipart20200908-4-1mqab9e_html_c1bde9edc8a2c9d3.png)

1. Make sure students can associate an action they take in lab to a process illustrated in the whiteboard diagram you draw for them

    1. How is PKI used?
    1. Secure websites with HTTPS

![](RackMultipart20200908-4-1mqab9e_html_8a0f5a99a6106aa4.png)

        1. Discuss why is HTTPS so important to have on all public-facing webservers
          1. HTTP is cleartext data transmission between you and the server
            1. Glaring reminder that the internet was not designed for security purposes
          2. HTTPS is easy to implement so why not?
          3. Increase end-user confidence in web server security = better experience on your website
          4. Good for defending against MITM and session hijacking although not a perfect defense
        2. Why don't all sites use HTTPS?
          1. Show students the [Why No HTTPS](https://www.troyhunt.com/why-no-https-heres-the-worlds-largest-websites-not-redirecting-insecure-requests/) site
          2. Example: Navigate to Boeing.com (or any site without HTTPS but obviously should have it)
            1. The lack of HTTPS can lead to negative press about your brand
            2. If a company fails to implement a simple protocol like HTTPS, this does not inspire public confidence in the org's security policies and capabilities
            3. Do your company a favor and champion HTTPS
        3. How to protect yourself
          1. HTTPSONLY browser addon
        4. How to install HTTPS on a web site you develop
          1. [Google Developer Article - How to Set up HTTPS](https://developers.google.com/web/fundamentals/security/encrypt-in-transit/enable-https)
      1. Certificates
        1. Windows Server supports CA and certificate assignment
        2. OpenSSL
      2. Authenticating users and computers with SSH (ref. [AWS SSH](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AccessingInstancesLinux.html))
      3. Email signing and encryption using Pretty Good Privacy (PGP)
        1. OpenPGP is the most current version
          1. Original PGP developed in the 90s
        2. Backwards compatibility means possibility of downgrade attack
        3. PGP is largely considered an insecure encryption method today but sees widespread use
      4. Example use case for PKI certificates
        1. Your organization is subject to export compliance regulation by the US government. The compliance officer must submit export compliance reports regularly to DECCS, but her computer is prompting for a certificate to validate her identity. Research DECCS policy and diagram the process. (Solution: [DECCS FAQ](https://www.pmddtc.state.gov/deccs?id=ddtc_public_portal_faq_detail&sys_id=fd856da2db5a2700529d368d7c9619fa))

  1. Lab
    1. Today's lab will arm students with two open-source, free, robust tools that are brand-agnostic. This means that graduates of our program who encounter a need for one of the below functionalities will not feel pressured into purchasing a product, but will instead have a toolkit ready for the job, and immediately be prepared to use those tools.
    2. OpenPGP
      1. Deploy [OpenPGP](https://www.openpgp.org/) to the computer you use email from
      2. Encrypt an email using OpenPGP
      3. Decrypt an email using OpenPGP

    3. OpenSSL
      1. Deploy OpenSSL to your Ubuntu Linux VM
      2. OpenSSL can be used for a wide range of data security needs as documented in [this article](https://prefetch.net/articles/realworldssl.html)
        1. Encryption and decryption
          1. Encrypt a file with OpenSSL
          2. Decrypt a file with OpenSSL
        2. Fingerprinting a file or directory of files
          1. Fingerprint a single file
          2. Fingerprint an entire directory of files
        3. Generating password file entries
        4. Digital certificates
          1. Create a CA, sign and issue certificates using [OpenSSL](https://pki-tutorial.readthedocs.io/en/latest/) certificate tutorial
            1. The tutorial provides three labs. All students should complete the Simple lab first, then advance as far as they can.
              1. Simple
              2. Advanced
              3. Expert
        5. Convert a DER to a PEM certificate type, or vice versa
        6. Monitor secure web server activity using HTTP GET request
          1. Create a script that automatically checks a website is properly handling SSL requests
          2. [Solution](https://github.com/Matty9191/misc-shell-scripts/blob/master/ssl-service-check)
        7. Check for expired web certificates
          1. Create a script that automatically checks if a SSL certificate for a website is about to expire, and notifies admin
          2. [Solution](https://github.com/Matty9191/ssl-cert-check)
      3. Stretch goal - Windows Server proprietary CA implementation
        1. Deploy Windows CA service on your Windows Server
        2. Generate a signed certificate
        3. Assign certificate to a domained computer
      4. Stretch goal - Add HTTPS to a website that doesn't have it yet
        1. [Solution](https://developers.google.com/web/fundamentals/security/encrypt-in-transit/enable-https)
      5. Fun - Install HTTPSONLY to your web browser and navigate to a non-HTTP website
      6. Stretch goal - Learn how to use encryption keys on AWS Cloud
        1. 50 mins - [Introduction to AWS Key Management Service](https://amazon.qwiklabs.com/focuses/10388?catalog_rank=%7B%22rank%22%3A3%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=5201321)
          1. Topics:
            1. Create an Encryption Key
            2. Create an S3 bucket with CloudTrail logging functions
            3. Encrypt data stored in a S3 bucket using an encryption key
            4. Monitor encryption key usage using CloudTrail
            5. Manage encryption keys for users and roles

1.
