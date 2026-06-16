# Cryptography — Final Exam Study Notes
# គ្រីបតូក្រាហ្វី — កំណត់ត្រាត្រៀមប្រឡងបញ្ចប់

> Reference / ឯកសារយោង: https://www.geeksforgeeks.org/computer-networks/cryptography-introduction/

---

## Question 1 — What is Cryptography?
## សំណួរទី ១ — តើគ្រីបតូក្រាហ្វី (Cryptography) ជាអ្វី?

### 🇬🇧 English

Cryptography is a way of keeping information safe by turning it into a secret, unreadable form, so that only the right person can read it.

Think of it like sending a letter in a locked box. Even if someone grabs the box on the way, they can't open it — only the person with the correct key can. Cryptography does the same thing with digital messages: it scrambles them so strangers can't understand them, and unscrambles them for the person who is allowed to read them.

The word comes from Greek: *kryptos* means "hidden" and *graphein* means "to write" — so cryptography literally means "hidden writing." We use it every day to protect things like passwords, bank transactions, and private messages.

### 🇰🇭 ភាសាខ្មែរ

គ្រីបតូក្រាហ្វី គឺជាវិធីការពារព័ត៌មាន ដោយប្ដូរវាទៅជាទម្រង់សម្ងាត់ដែលអានមិនបាន ដើម្បីឲ្យតែអ្នកដែលមានសិទ្ធិប៉ុណ្ណោះ អាចអានវាបាន។

ស្រមៃថាវាដូចជាការផ្ញើសំបុត្រនៅក្នុងប្រអប់ដែលជាប់សោ។ ទោះបីមាននរណាម្នាក់ឆក់យកប្រអប់នេះនៅតាមផ្លូវក៏ដោយ ក៏គេមិនអាចបើកវាបានដែរ — មានតែអ្នកដែលមានកូនសោត្រឹមត្រូវប៉ុណ្ណោះ ទើបបើកបាន។ គ្រីបតូក្រាហ្វីក៏ធ្វើបែបនេះដែរ ចំពោះសារឌីជីថល៖ វាបំប្លែងសារឲ្យច្របូកច្របល់ ដើម្បីកុំឲ្យអ្នកក្រៅអាចយល់បាន ហើយប្ដូរវាមកវិញសម្រាប់អ្នកដែលមានសិទ្ធិអាន។

ពាក្យនេះមកពីភាសាក្រិក៖ *kryptos* មានន័យថា «លាក់» និង *graphein* មានន័យថា «សរសេរ» — ដូច្នេះ គ្រីបតូក្រាហ្វី មានន័យត្រង់ៗថា «ការសរសេរលាក់»។ យើងប្រើវាជារៀងរាល់ថ្ងៃ ដើម្បីការពារ ពាក្យសម្ងាត់ ប្រតិបត្តិការធនាគារ និងសារផ្ទាល់ខ្លួន។

---

## Question 2 — Core Principles of Cryptography
## សំណួរទី ២ — គោលការណ៍សំខាន់ៗនៃគ្រីបតូក្រាហ្វី

### 🇬🇧 English

Cryptography is built on **four main principles**. An easy way to remember them is **C – I – A – N**.

**1. Confidentiality (Keeping it private)**
Only the people who are allowed to see the information can see it. Everyone else is locked out. This is the main goal of encryption.

**2. Integrity (Keeping it unchanged)**
The data must stay correct and complete. If someone tries to change it secretly, we can detect that it was changed.

**3. Authentication (Proving who you are)**
It checks the identity of the sender and receiver — making sure the message really came from the person who claims to have sent it.

**4. Non-Repudiation (No denying it later)**
The sender cannot later say "I never sent that." There is proof that they really sent the message. (This is what a digital signature does.)

### 🇰🇭 ភាសាខ្មែរ

គ្រីបតូក្រាហ្វីត្រូវបានបង្កើតឡើងលើ **គោលការណ៍សំខាន់ៗចំនួន ៤**។ វិធីងាយចងចាំគឺ **C – I – A – N**។

**១. ការសម្ងាត់ (Confidentiality)**
មានតែអ្នកដែលមានសិទ្ធិប៉ុណ្ណោះ ទើបអាចមើលឃើញព័ត៌មាននោះ។ អ្នកផ្សេងទៀតទាំងអស់ត្រូវបានរារាំង។ នេះជាគោលដៅចម្បងនៃការអ៊ិនគ្រីប។

**២. ភាពត្រឹមត្រូវ (Integrity)**
ទិន្នន័យត្រូវតែនៅត្រឹមត្រូវ និងពេញលេញ។ ប្រសិនបើមាននរណាម្នាក់ព្យាយាមកែប្រែវាដោយលាក់កំបាំង យើងអាចរកឃើញថាវាត្រូវបានកែប្រែ។

**៣. ការផ្ទៀងផ្ទាត់អត្តសញ្ញាណ (Authentication)**
វាពិនិត្យអត្តសញ្ញាណរបស់អ្នកផ្ញើ និងអ្នកទទួល — ដើម្បីប្រាកដថាសារនោះពិតជាមកពីអ្នកដែលអះអាងថាបានផ្ញើពិតមែន។

**៤. ការមិនអាចបដិសេធបាន (Non-Repudiation)**
អ្នកផ្ញើមិនអាចនិយាយពេលក្រោយថា «ខ្ញុំមិនដែលផ្ញើសារនោះទេ» បានឡើយ។ មានភស្តុតាងបញ្ជាក់ថាគេពិតជាបានផ្ញើសារនោះមែន។ (នេះជាមុខងាររបស់ហត្ថលេខាឌីជីថល។)

---

## Question 3 — How Cryptography Works? What is Ciphertext? What is Key?
## សំណួរទី ៣ — តើគ្រីបតូក្រាហ្វីដំណើរការយ៉ាងដូចម្ដេច? Ciphertext ជាអ្វី? Key ជាអ្វី?

### 🇬🇧 English

**How it works (step by step):**

1. We start with a normal, readable message — this is called **plaintext**.
2. We use an **encryption algorithm** together with a **key** to scramble it.
3. The scrambled, unreadable result is called **ciphertext**.
4. The receiver uses a key with a **decryption algorithm** to turn the ciphertext back into the original message.

**Simple flow:**
```
Plaintext  →  [ Encrypt + Key ]  →  Ciphertext  →  [ Decrypt + Key ]  →  Plaintext
```

**Key words to know:**

- **Plaintext** = the original readable message (for example: "Geeksforgeeks").
- **Ciphertext** = the scrambled, secret version of the message that no one can read without the key.
- **Key** = a secret piece of information (like a password made of numbers/letters) used to lock (encrypt) and unlock (decrypt) the message. Even if people know *how* the lock works, the message stays safe as long as the key is secret.

**Easy example — Caesar Cipher:**
Shift every letter forward by 3 positions. The word **"Geeksforgeeks"** becomes **"Jhhnvirujhhnv"**. Here, the number "3" is the key.

### 🇰🇭 ភាសាខ្មែរ

**របៀបដំណើរការ (ជាជំហានៗ):**

១. យើងចាប់ផ្ដើមដោយសារធម្មតាដែលអានបាន — នេះហៅថា **Plaintext (អត្ថបទច្បាស់)**។
២. យើងប្រើ **ក្បួនអ៊ិនគ្រីប (encryption algorithm)** រួមជាមួយ **កូនសោ (key)** ដើម្បីបំប្លែងវាឲ្យច្របូកច្របល់។
៣. លទ្ធផលដែលច្របូកច្របល់ និងអានមិនបាននោះ ហៅថា **Ciphertext (អត្ថបទសម្ងាត់)**។
៤. អ្នកទទួលប្រើកូនសោជាមួយ **ក្បួនឌិគ្រីប (decryption algorithm)** ដើម្បីប្ដូរ Ciphertext ត្រឡប់ទៅជាសារដើមវិញ។

**លំហូរសាមញ្ញ៖**
```
Plaintext  →  [ អ៊ិនគ្រីប + Key ]  →  Ciphertext  →  [ ឌិគ្រីប + Key ]  →  Plaintext
```

**ពាក្យសំខាន់ៗដែលត្រូវដឹង៖**

- **Plaintext** = សារដើមដែលអានបាន (ឧទាហរណ៍៖ "Geeksforgeeks")។
- **Ciphertext** = ទម្រង់សម្ងាត់នៃសារ ដែលច្របូកច្របល់ ហើយគ្មាននរណាអានបានទេ បើគ្មានកូនសោ។
- **Key (កូនសោ)** = ព័ត៌មានសម្ងាត់មួយ (ដូចជាពាក្យសម្ងាត់ដែលធ្វើពីលេខ/អក្សរ) ប្រើសម្រាប់ចាក់សោ (អ៊ិនគ្រីប) និងបើកសោ (ឌិគ្រីប) សារ។ ទោះបីមនុស្សដឹងពី *របៀប* ដែលសោដំណើរការក៏ដោយ ក៏សារនៅតែសុវត្ថិភាពដែរ ដរាបណាកូនសោនៅសម្ងាត់។

**ឧទាហរណ៍ងាយយល់ — Caesar Cipher:**
ផ្លាស់ប្ដូរអក្សរនីមួយៗទៅមុខ ៣ ខ្ទង់។ ពាក្យ **"Geeksforgeeks"** ក្លាយទៅជា **"Jhhnvirujhhnv"**។ ត្រង់នេះ លេខ "៣" គឺជាកូនសោ។

---

## Question 4 — Types of Cryptography (Explained One by One)
## សំណួរទី ៤ — ប្រភេទនៃគ្រីបតូក្រាហ្វី (ពន្យល់ម្ដងមួយៗ)

### 🇬🇧 English

There are **three main types** of cryptography.

**Type 1: Symmetric-Key Cryptography (Secret-Key)**
- Uses **one single key** for both locking (encrypting) and unlocking (decrypting).
- Both the sender and receiver must share the **same secret key**.
- **Good:** It is very fast, great for large amounts of data.
- **Problem:** You must find a safe way to share the key. If someone steals the key, your security is broken.
- **Examples:** AES, DES.
- *Think of it like:* one key that both people use for the same lock.

**Type 2: Asymmetric-Key Cryptography (Public-Key)**
- Uses **two keys that work as a pair**: a **public key** and a **private key**.
- The **public key** is shared with everyone and used to encrypt (lock) the message.
- The **private key** is kept secret and is the only key that can decrypt (unlock) it.
- **Good:** More secure — you don't need to share a secret key. It also allows digital signatures.
- **Problem:** It is slower than symmetric cryptography.
- **Example:** RSA.
- *Think of it like:* a mailbox — anyone can drop a letter in (public key), but only you have the key to open it (private key).

**Type 3: Hash Functions**
- Takes data of **any size** and turns it into a **fixed-length code** called a hash (or digest).
- It uses **no key** and is **one-way** — you can never turn the hash back into the original data.
- **Used for:** checking data integrity (if one tiny part of the data changes, the hash changes completely) and storing passwords safely.
- **Example:** SHA-256.
- *Think of it like:* a fingerprint for data — unique, and you can't rebuild the person from the fingerprint.

**Quick Comparison Table**

| Type | Keys used | Speed | Reversible? | Example |
|------|-----------|-------|-------------|---------|
| Symmetric | One shared key | Fast | Yes | AES, DES |
| Asymmetric | Public + Private | Slower | Yes | RSA |
| Hash function | No key | Fast | No (one-way) | SHA-256 |

### 🇰🇭 ភាសាខ្មែរ

គ្រីបតូក្រាហ្វីមាន **ប្រភេទសំខាន់ៗ ៣**។

**ប្រភេទទី ១៖ Symmetric-Key Cryptography (កូនសោសម្ងាត់រួម)**
- ប្រើ **កូនសោតែមួយ** សម្រាប់ទាំងការអ៊ិនគ្រីប និងឌិគ្រីប។
- ទាំងអ្នកផ្ញើ និងអ្នកទទួល ត្រូវតែប្រើ **កូនសោសម្ងាត់ដូចគ្នា**។
- **ល្អ៖** វាលឿនណាស់ ស័ក្តិសមសម្រាប់ទិន្នន័យច្រើន។
- **បញ្ហា៖** អ្នកត្រូវរកវិធីសុវត្ថិភាពដើម្បីចែករំលែកកូនសោ។ បើមាននរណាលួចកូនសោបាន សុវត្ថិភាពនឹងបាក់។
- **ឧទាហរណ៍៖** AES, DES។
- *ស្រមៃថា៖* កូនសោតែមួយដែលមនុស្សពីរនាក់ប្រើជាមួយសោតែមួយ។

**ប្រភេទទី ២៖ Asymmetric-Key Cryptography (កូនសោសាធារណៈ)**
- ប្រើ **កូនសោពីរដែលដំណើរការជាគូ**៖ **កូនសោសាធារណៈ (public key)** និង **កូនសោឯកជន (private key)**។
- **កូនសោសាធារណៈ** ត្រូវបានចែករំលែកជាមួយមនុស្សគ្រប់គ្នា ហើយប្រើសម្រាប់អ៊ិនគ្រីប (ចាក់សោ) សារ។
- **កូនសោឯកជន** ត្រូវរក្សាទុកជាសម្ងាត់ ហើយជាកូនសោតែមួយគត់ដែលអាចឌិគ្រីប (បើកសោ) វាបាន។
- **ល្អ៖** សុវត្ថិភាពជាង — មិនចាំបាច់ចែករំលែកកូនសោសម្ងាត់ទេ។ វាក៏អនុញ្ញាតឲ្យមានហត្ថលេខាឌីជីថលផងដែរ។
- **បញ្ហា៖** វាយឺតជាង Symmetric។
- **ឧទាហរណ៍៖** RSA។
- *ស្រមៃថា៖* ប្រអប់សំបុត្រ — នរណាក៏អាចដាក់សំបុត្រចូលបាន (កូនសោសាធារណៈ) ប៉ុន្តែមានតែអ្នកប៉ុណ្ណោះដែលមានកូនសោបើកវា (កូនសោឯកជន)។

**ប្រភេទទី ៣៖ Hash Functions (មុខងារ Hash)**
- ទទួលយកទិន្នន័យ **ទំហំណាក៏បាន** ហើយប្ដូរវាទៅជា **កូដប្រវែងថេរ** ហៅថា hash (ឬ digest)។
- វា **មិនប្រើកូនសោ** ហើយ **ដំណើរការតែមួយទិស** — អ្នកមិនអាចប្ដូរ hash ត្រឡប់ទៅជាទិន្នន័យដើមវិញបានឡើយ។
- **ប្រើសម្រាប់៖** ពិនិត្យភាពត្រឹមត្រូវនៃទិន្នន័យ (បើផ្នែកតូចមួយនៃទិន្នន័យផ្លាស់ប្ដូរ hash នឹងផ្លាស់ប្ដូរទាំងស្រុង) និងរក្សាទុកពាក្យសម្ងាត់ដោយសុវត្ថិភាព។
- **ឧទាហរណ៍៖** SHA-256។
- *ស្រមៃថា៖* ស្នាមម្រាមដៃសម្រាប់ទិន្នន័យ — មានតែមួយគត់ ហើយអ្នកមិនអាចបង្កើតមនុស្សឡើងវិញពីស្នាមម្រាមដៃបានទេ។

**តារាងប្រៀបធៀបរហ័ស**

| ប្រភេទ | កូនសោប្រើ | ល្បឿន | ប្ដូរវិញបានទេ? | ឧទាហរណ៍ |
|--------|-----------|--------|----------------|----------|
| Symmetric | កូនសោរួមមួយ | លឿន | បាន | AES, DES |
| Asymmetric | សាធារណៈ + ឯកជន | យឺតជាង | បាន | RSA |
| Hash function | គ្មានកូនសោ | លឿន | មិនបាន (មួយទិស) | SHA-256 |

---

## Applications of Cryptography / ការអនុវត្តន៍នៃគ្រីបតូក្រាហ្វី

- 🏦 Secure online banking and e-commerce / ធនាគារអនឡាញ និងពាណិជ្ជកម្មអេឡិចត្រូនិកដោយសុវត្ថិភាព
- ✍️ Digital signatures for documents / ហត្ថលេខាឌីជីថលសម្រាប់ឯកសារ
- 🔑 Password protection / ការការពារពាក្យសម្ងាត់
- 🪖 Military and intelligence communications / ការទំនាក់ទំនងយោធា និងស៊ើបការណ៍សម្ងាត់

---

*Source / ប្រភព: GeeksforGeeks — Cryptography Introduction*
*https://www.geeksforgeeks.org/computer-networks/cryptography-introduction/*
