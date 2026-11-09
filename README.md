# Cybersecurity, Law and Ethics (CSE487)

Coursework from my BSc in Computer Science and Engineering at East West University, Dhaka, in Spring 2024. Both mini projects were done in a group of four. One is a hands-on security lab and the other is a policy comparison.

## Mini Project 1: Securing a networked system with Public Key Infrastructure

We set up our own small certificate authority hierarchy on an Ubuntu 18.04 virtual machine and used it to put HTTPS on a local web server. The report walks through every command with screenshots, and it links to a demo video.

What we built, step by step:

1. **A root CA and a sub-CA.** Each has its own directory structure, index and serial files, and an AES-256 encrypted 4096-bit RSA private key. The root certificate is valid for 7,305 days, and the sub-CA certificate, signed by the root, for 3,652 days.
2. **A server certificate.** The server has a 2048-bit RSA key. Its certificate request was signed by the sub-CA and is valid for 365 days.
3. **A secured Apache server.** In XAMPP, the SSL config points at the server certificate and key. A hosts entry maps `www.verysecureserver.com` to a local address.
4. **Browser trust.** We imported the root and sub-CA certificates into Firefox, so the browser accepts the site.

The tools were a virtual machine, Ubuntu 18.04, XAMPP, OpenSSL and Firefox 59.0.2. The report is 16 pages, and the 24-slide deck covers the same steps.

## Mini Project 2: Privacy policies of Bangladeshi clothing brands

This is a one-page poster titled "Clothing Companies Approaches to Privacy Policies, Regulations, and Laws in Bangladesh". We read the public privacy policies of four brands (Aarong, Sailor, Yellow and Richman) and compared them on:

- what personal data they collect and what they use it for
- whether they share or sell it
- whether customers can access, change or delete their data, and opt out
- social media and third-party platforms
- analytics, log files and cookies
- children's privacy under COPPA

The poster concludes that Sailor was the most transparent of the four. It's a comparison of what each policy page said when we read it, not legal advice. The sources are listed on the poster.

## What's in the repo

- `miniProject1CSE487.pdf`: the PKI lab report
- `Presentation.pptx`: the 24-slide presentation for the PKI lab
- `MiniProject_2(Poster).pdf`: the privacy policy poster

## Please don't copy

This is my own coursework, shared for my portfolio. Please don't submit it as yours. If it helps your thinking, cite it.

## Contact

- GitHub: [Zarin2000](https://github.com/Zarin2000)
- LinkedIn: [Zarin Tasnim Nuzhat](https://www.linkedin.com/in/zarin-tasnim-nuzhat-829007202)
- ORCID: [0009-0006-3469-1876](https://orcid.org/0009-0006-3469-1876)
