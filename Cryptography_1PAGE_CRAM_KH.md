# Cryptography — សន្លឹកសង្ខេប ១ ទំព័រ (ភាសាខ្មែរ)

## គន្លឹះធំ
សំណួរ ១៥ ភាគច្រើនកើតចេញពីគំនិតស្នូលពីរបី + ឧទាហរណ៍ **HELLO→KHOOR** តែមួយ។ រៀនគំនិតស្នូល រួចរៀន **ពាក្យគន្លឹះ** សម្រាប់សំណួរនីមួយៗ។ ពិន្ទុមកពី **ចំណុច** មិនមែនពាក្យពិតប្រាកដ។

> ពាក្យបច្ចេកទេស (AES, RSA, SHA-256, HTTPS, TLS) រក្សាជាភាសាអង់គ្លេស ព្រោះអ្នកសរសេរវាក្នុងវិញ្ញាសាអង់គ្លេស។

---

## ផ្នែកទី ១ — គំនិតស្នូល (រៀនមុនគេ — អានឱ្យឮៗ)

- **CIAN** = សេវាសុវត្ថិភាព ៤ → **C**onfidentiality (សម្ងាត់) · **I**ntegrity (ត្រឹមត្រូវ) · **A**uthentication (ផ្ទៀងផ្ទាត់) · **N**on-repudiation (មិនអាចបដិសេធ)
- **ឧទាហរណ៍មាស HELLO→KHOOR** (Caesar shift +3) → ប្រើបាននៅ Q3, Q9, Q10 (encrypt/decrypt, plaintext/ciphertext, cipher)
- **Plaintext** = អត្ថបទដើមអានបាន (HELLO) · **Ciphertext** = អត្ថបទច្របល់ (KHOOR)
- **Encryption** = plaintext→ciphertext (ត្រូវ key) · **Decryption** = ciphertext→plaintext
- **Symmetric** = key **១** រួមគ្នា (AES) · **Asymmetric** = key **២** គូ public+private (RSA)
- **Hashing** = មួយទិស, គ្មាន key, ប្រវែងថេរ, integrity (SHA-256) · **Encryption** = ពីរទិស, មាន key, confidentiality
- **Kerckhoffs** = សុវត្ថិភាពពឹងលើ **key** សម្ងាត់ មិនមែន algorithm

---

## ផ្នែកទី ២ — ពាក្យគន្លឹះ ១៥ សំណួរ

1. Cryptography ជាអ្វី = វិទ្យាសាស្ត្រការពារព័ត៌មាន (hidden writing); ប្រើ៖ HTTPS, messaging, passwords, Wi-Fi
2. គោលការណ៍ស្នូល = **CIAN** (Confidentiality, Integrity, Authentication, Non-repudiation)
3. Encryption/Decryption = plaintext↔ciphertext ត្រូវ key; គោលដៅ=សម្ងាត់; **ឧទាហរណ៍ HELLO→KHOOR** (shift 3); AES ទំនើប
4. Key + ហេតុអ្វីសម្ងាត់ (symmetric) = key=តម្លៃសម្ងាត់គ្រប់គ្រង; symmetric key ដូចគ្នា→បើលេច បាត់សម្ងាត់ទាំងអស់; **Kerckhoffs**
5. Data integrity + tool = ទិន្នន័យមិនកែ/ខូច; ឧបករណ៍ = **hash function (SHA-256)** ប្រៀបធៀប hash
6. Brute-force = សាកល្បង key/password **គ្រប់បន្សំ** រហូតត្រូវ; ពឹងលើ **key space**; key វែង→មិនអាច
7. Hashing ធៀប Encryption = តារាង៖ មួយទិស/ពីរទិស, គ្មាន key/មាន key, integrity/confidentiality
8. Active ធៀប Passive = Passive=ស្ដាប់តែ (sniffing, ពិបាករកឃើញ, ការពារដោយ encryption); Active=កែ/រំខាន (MITM, replay, DoS, ការពារដោយ authentication)
9. Plaintext ធៀប Ciphertext = ដើមអានបាន (HELLO) ធៀប ច្របល់អានមិនបាន (KHOOR)
10. Cipher = algorithm encrypt/decrypt; **ឧទាហរណ៍បុរាណ = Caesar** (substitution); ផ្សេង៖ Vigenère, transposition
11. Password reuse + crypto ជួយ = reuse→credential stuffing (breach មួយ បាត់ទាំងអស់); ជួយ៖ hashing+salting, password manager, MFA
12. Digital certificate (HTTPS) = ឯកសារចេញដោយ **CA** ភ្ជាប់អត្តសញ្ញាណ→public key; គោលដៅ៖ ① authentication/trust ② ផ្ដល់ public key (TLS); ឆ្លើយ "តើគេហទំព័រនេះពិតឬ?"
13. Symmetric ធៀប Asymmetric = symmetric=key១រួម (AES); asymmetric=key២គូ public+private (RSA)
14. Alice→Bob key ណា? = **public key របស់ Bob**; ព្រោះតែ private key របស់ Bob ឌិគ្រីបបាន→សម្ងាត់; ច្បាប់មេដៃ៖ encrypt ដោយ public key អ្នកទទួល
15. Steganography ធៀប Cryptography = Stego=លាក់ **អត្ថិភាព** (ក្នុងរូបភាព/pixels); Crypto=លាក់ **អត្ថន័យ**; អាចបញ្ចូលគ្នា

---

## ផ្លូវកាត់៖ ចម្លើយប្រើឡើងវិញ
- **HELLO→KHOOR** ប្រើបាននៅ Q3, Q9, Q10 — រៀនម្ដងឆ្លើយ ៣
- **CIAN** ប្រើនៅ Q1, Q2 · **key/symmetric-asymmetric** ប្រើនៅ Q4, Q13, Q14
- **hash/integrity** ប្រើនៅ Q5, Q7
→ ពិតប្រាកដមានរឿងត្រូវរៀនតែប្រហែល **៧-៨** មិនមែន ១៥ ទេ។

---

## ផែនការសិក្សា & ច្បាប់
1. **ម៉ោង ១** — ទន្ទេញ **CIAN**, **HELLO→KHOOR**, symmetric/asymmetric, hashing/encryption ឱ្យឮៗ
2. **ម៉ោង ២** — អានសំណួរ → និយាយពាក្យគន្លឹះ → និយាយចម្លើយ → ពិនិត្យ
3. **ម៉ោង ៣** — សាកល្បងតែសំណួរដែលខុស + សរសេរ ៣ ចម្លើយលើក្រដាស
4. **ម៉ោង ៤** — អានម្ដងទៀត រួចគេង
- **និយាយឱ្យឮ** · **ពិន្ទុមកពីចំណុច** · សរសេរ **bullet points** · ចាំ **HELLO→KHOOR** (វាជួយឆ្លើយ ៣ សំណួរ) · ចាំ **Alice→public key របស់ Bob**
