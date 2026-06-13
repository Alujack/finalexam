# Introduction to Cryptography — Model Answers (English + ខ្មែរ)

*Model answers / ចម្លើយគំរូ. Proper nouns and technical terms (AES, RSA, SHA-256, HTTPS, TLS, HMAC, etc.) kept in Latin script. / នាមជាក់លាក់ និងពាក្យបច្ចេកទេស (AES, RSA, SHA-256, HTTPS, TLS, HMAC ។ល។) រក្សាជាអក្សរឡាតាំង។*

---

### 1) What is cryptography, and what is its main purpose in daily digital life? / តើ cryptography ជាអ្វី ហើយគោលបំណងសំខាន់របស់វាក្នុងជីវិតឌីជីថលប្រចាំថ្ងៃជាអ្វី?

**English:**
- **Cryptography** = the science of securing information and communication using mathematical techniques, so only authorised parties can read or use it. (From the Greek for "hidden writing.")
- **Main purpose in daily life:** protect the **confidentiality, integrity, and authenticity** of data in an open, untrusted environment like the internet. You rely on it constantly without noticing:
  - **HTTPS** secures websites (online banking, shopping, logins).
  - **Messaging apps** (WhatsApp, Signal) use end-to-end encryption so only you and the recipient can read messages.
  - **Passwords** are stored as hashes, not plaintext.
  - **Wi-Fi (WPA), bank cards/PINs, and digital signatures** all depend on cryptography.
- In short, cryptography is what makes it safe to send private and valuable information across networks we don't control.

**ខ្មែរ:**
- **Cryptography** = វិទ្យាសាស្ត្រនៃការការពារព័ត៌មាន និងទំនាក់ទំនង ដោយប្រើបច្ចេកទេសគណិតវិទ្យា ដើម្បីឱ្យតែភាគីមានសិទ្ធិអាច អាន ឬប្រើ។ (មកពីភាសាក្រិក "ការសរសេរលាក់"។)
- **គោលបំណងសំខាន់ក្នុងជីវិតប្រចាំថ្ងៃ៖** ការពារ **ការសម្ងាត់ ភាពត្រឹមត្រូវ និងភាពពិត** នៃទិន្នន័យ ក្នុងបរិស្ថានបើកចំហ និងមិនជឿទុកចិត្តដូចជាអ៊ីនធឺណិត។ អ្នកពឹងលើវាជានិច្ច ដោយមិនដឹងខ្លួន៖
  - **HTTPS** ការពារគេហទំព័រ (ធនាគារអនឡាញ ការទិញ ការចូលគណនី)។
  - **កម្មវិធីផ្ញើសារ** (WhatsApp, Signal) ប្រើ end-to-end encryption ឱ្យតែអ្នក និងអ្នកទទួលអានសារបាន។
  - **ពាក្យសម្ងាត់** ត្រូវផ្ទុកជា hash មិនមែនជាអក្សរធម្មតា។
  - **Wi-Fi (WPA), កាតធនាគារ/PIN និងហត្ថលេខាឌីជីថល** ទាំងអស់ពឹងលើ cryptography។
- សរុប cryptography ជាអ្វីដែលធ្វើឱ្យមានសុវត្ថិភាពក្នុងការផ្ញើព័ត៌មានឯកជន និងមានតម្លៃ ឆ្លងបណ្ដាញដែលយើងមិនគ្រប់គ្រង។

### 2) What are the core principles of cryptography? / តើគោលការណ៍ស្នូលនៃ cryptography ជាអ្វី?

**English:**
- The four **security services** cryptography provides:
  - **Confidentiality** — keeping information secret from unauthorised parties (via encryption).
  - **Integrity** — ensuring data has not been altered or tampered with (via hash functions and MACs).
  - **Authentication** — verifying the identity of a user or the origin of a message.
  - **Non-repudiation** — preventing a sender from later denying they sent a message (via digital signatures).
- (Access control and availability are sometimes added as supporting goals.)

**ខ្មែរ:**
- សេវាសុវត្ថិភាព ៤ ដែល cryptography ផ្ដល់៖
  - **ការសម្ងាត់ (Confidentiality)** — រក្សាព័ត៌មានសម្ងាត់ពីភាគីគ្មានសិទ្ធិ (តាមការអ៊ិនគ្រីប)។
  - **ភាពត្រឹមត្រូវ (Integrity)** — ធានាថាទិន្នន័យមិនត្រូវកែ ឬប៉ះពាល់ (តាម hash functions និង MACs)។
  - **ការផ្ទៀងផ្ទាត់ (Authentication)** — ផ្ទៀងផ្ទាត់អត្តសញ្ញាណអ្នកប្រើ ឬប្រភពនៃសារ។
  - **ការមិនអាចបដិសេធ (Non-repudiation)** — ការពារអ្នកផ្ញើពីការបដិសេធក្រោយមកថាបានផ្ញើសារ (តាមហត្ថលេខាឌីជីថល)។
- (ការគ្រប់គ្រងការចូល និងភាពអាចប្រើបាន ពេលខ្លះបន្ថែមជាគោលដៅគាំទ្រ។)

### 3) Explain in detail Encryption and Decryption. Give an example. / ពន្យល់លម្អិតពី Encryption និង Decryption។ ផ្ដល់ឧទាហរណ៍។

**English:**
- **Encryption** = converting readable data (**plaintext**) into an unreadable form (**ciphertext**) using an algorithm and a **key**.
- **Decryption** = the reverse — converting ciphertext back into the original plaintext using the correct key.
  - `Plaintext --[ Encrypt with key ]--> Ciphertext`
  - `Ciphertext --[ Decrypt with key ]--> Plaintext`
- **Purpose:** confidentiality — even if an attacker intercepts the ciphertext, they can't read it without the key.
- **Example (Caesar cipher, shift of 3):** each letter shifts three places forward.
  - Plaintext: `HELLO`
  - Encryption (+3): H→K, E→H, L→O, L→O, O→R → Ciphertext: `KHOOR`
  - Decryption (−3): `KHOOR` → `HELLO`
- Here the "algorithm" is *shift the letters* and the "key" is the *number 3*. Modern algorithms like **AES** work on the same principle but with far more complex mathematics on bits.

**ខ្មែរ:**
- **Encryption** = ការបម្លែងទិន្នន័យអាចអានបាន (**plaintext**) ទៅជាទម្រង់អានមិនបាន (**ciphertext**) ដោយប្រើ algorithm និង **key**។
- **Decryption** = ដំណើរការបញ្ច្រាស — បម្លែង ciphertext ត្រឡប់ទៅ plaintext ដើម ដោយប្រើ key ត្រឹមត្រូវ។
  - `Plaintext --[ អ៊ិនគ្រីបដោយ key ]--> Ciphertext`
  - `Ciphertext --[ ឌិគ្រីបដោយ key ]--> Plaintext`
- **គោលបំណង៖** ការសម្ងាត់ — ទោះអ្នកវាយប្រហារចាប់យក ciphertext ក៏អានមិនបានដែរ បើគ្មាន key។
- **ឧទាហរណ៍ (Caesar cipher ផ្លាស់ ៣)៖** អក្សរនីមួយៗផ្លាស់បីកន្លែងទៅមុខ។
  - Plaintext៖ `HELLO`
  - Encryption (+3)៖ H→K, E→H, L→O, L→O, O→R → Ciphertext៖ `KHOOR`
  - Decryption (−3)៖ `KHOOR` → `HELLO`
- នៅទីនេះ "algorithm" គឺ *ផ្លាស់អក្សរ* ហើយ "key" គឺ *លេខ ៣*។ Algorithm ទំនើបដូច **AES** ដំណើរការលើគោលការណ៍ដូចគ្នា ប៉ុន្តែជាមួយគណិតវិទ្យាស្មុគស្មាញជាងលើ bits។

### 4) What is a "key" in cryptography, and why must it be kept secret in symmetric systems? / តើ "key" ក្នុង cryptography ជាអ្វី ហើយហេតុអ្វីត្រូវរក្សាសម្ងាត់ក្នុងប្រព័ន្ធ symmetric?

**English:**
- A **key** is a secret value (a string of bits) that controls encryption and decryption. The same algorithm with different keys produces different ciphertext, and only the correct key can reverse the encryption.
- In a **symmetric system**, the **same key** is used to both encrypt *and* decrypt. So anyone who obtains the key can decrypt every message protected by it — if it leaks, all confidentiality is lost. It must be kept strictly secret and shared only through a secure channel.
- This reflects **Kerckhoffs's principle:** the security of a system should depend only on the secrecy of the **key**, not the secrecy of the algorithm (which can be public). The key is the single most important secret in the system.

**ខ្មែរ:**
- **Key** ជាតម្លៃសម្ងាត់ (ខ្សែ bits) ដែលគ្រប់គ្រងការអ៊ិនគ្រីប និងឌិគ្រីប។ Algorithm ដូចគ្នាជាមួយ key ផ្សេងគ្នា ផលិត ciphertext ផ្សេងគ្នា ហើយតែ key ត្រឹមត្រូវប៉ុណ្ណោះអាចបញ្ច្រាសការអ៊ិនគ្រីប។
- ក្នុង **ប្រព័ន្ធ symmetric** **key ដូចគ្នា** ត្រូវប្រើទាំងអ៊ិនគ្រីប *និង* ឌិគ្រីប។ ដូច្នេះអ្នកណាដែលទទួល key អាចឌិគ្រីបរាល់សារដែលវាការពារ — បើវាលេចធ្លាយ ការសម្ងាត់ទាំងអស់បាត់បង់។ វាត្រូវរក្សាសម្ងាត់យ៉ាងតឹងរ៉ឹង និងចែករំលែកតែតាមបណ្ដាញសុវត្ថិភាព។
- នេះឆ្លុះបញ្ចាំង **គោលការណ៍ Kerckhoffs៖** សុវត្ថិភាពប្រព័ន្ធគួរពឹងតែលើការសម្ងាត់នៃ **key** មិនមែនការសម្ងាត់នៃ algorithm (ដែលអាចជាសាធារណៈ)។ Key ជាការសម្ងាត់សំខាន់បំផុតតែមួយក្នុងប្រព័ន្ធ។

### 5) Explain "data integrity" and name one cryptographic tool used to verify it. / ពន្យល់ "data integrity" និងដាក់ឈ្មោះឧបករណ៍ cryptography មួយដែលប្រើផ្ទៀងផ្ទាត់វា។

**English:**
- **Data integrity** = the assurance that data has **not been altered, corrupted, or tampered with** — whether accidentally (transmission errors) or maliciously (an attacker) — between creation/sending and receipt/use. Integrity does *not* keep data secret; it guarantees the data is unchanged and trustworthy.
- **Cryptographic tool:** a **cryptographic hash function** (e.g. SHA-256). The sender computes a hash (a fixed-length "fingerprint") and shares it; the receiver re-computes the hash of the received data and compares. If the two match, the data is intact; if even one bit changed, the hash differs.
- (MACs/HMACs and digital signatures provide integrity *plus* authentication.)

**ខ្មែរ:**
- **Data integrity** = ការធានាថាទិន្នន័យ **មិនត្រូវកែ ខូច ឬប៉ះពាល់** — ទោះដោយចៃដន្យ (កំហុសបញ្ជូន) ឬដោយចេតនា (អ្នកវាយប្រហារ) — រវាងពេលបង្កើត/ផ្ញើ និងពេលទទួល/ប្រើ។ Integrity *មិន* រក្សាទិន្នន័យសម្ងាត់ទេ៖ វាធានាថាទិន្នន័យមិនផ្លាស់ប្ដូរ និងគួរឱ្យទុកចិត្ត។
- **ឧបករណ៍ cryptography៖** **cryptographic hash function** (ឧ. SHA-256)។ អ្នកផ្ញើគណនា hash ("ស្នាមម្រាមដៃ" ប្រវែងថេរ) ហើយចែករំលែក៖ អ្នកទទួលគណនា hash នៃទិន្នន័យឡើងវិញ ហើយប្រៀបធៀប។ បើទាំងពីរត្រូវគ្នា ទិន្នន័យនៅដដែល៖ បើ bit តែមួយផ្លាស់ប្ដូរ hash នឹងខុស។
- (MACs/HMACs និងហត្ថលេខាឌីជីថល ផ្ដល់ integrity *បូក* ការផ្ទៀងផ្ទាត់។)

### 6) What does "brute-force attack" mean in simple terms? / តើ "brute-force attack" មានន័យយ៉ាងណាក្នុងន័យសាមញ្ញ?

**English:**
- A **brute-force attack** = simply **trying every possible key or password, one after another, until the correct one is found**. No cleverness — just exhaustive guessing, usually automated at high speed.
- Analogy: a thief trying every combination on a padlock until it opens.
- Success depends entirely on the **size of the key space**: a short/simple key can be cracked quickly, but a long key (e.g. 256-bit AES) has so many combinations that trying them all would take longer than the age of the universe — making brute force infeasible.
- This is why **longer keys and strong passwords** matter.

**ខ្មែរ:**
- **Brute-force attack** = គ្រាន់តែ **សាកល្បង key ឬពាក្យសម្ងាត់ដែលអាចមានទាំងអស់ ម្ដងមួយៗ រហូតរក key ត្រឹមត្រូវ**។ គ្មានល្បិច — គ្រាន់តែការទាយដ៏ហត់នឿយ ជាទូទៅធ្វើស្វ័យប្រវត្តិក្នុងល្បឿនលឿន។
- ការប្រៀបធៀប៖ ចោរសាកល្បងគ្រប់បន្សំលើសោ រហូតវាបើក។
- ភាពជោគជ័យពឹងទាំងស្រុងលើ **ទំហំ key space**៖ key ខ្លី/សាមញ្ញ អាចបំបែកលឿន ប៉ុន្តែ key វែង (ឧ. AES 256-bit) មានបន្សំច្រើនណាស់ ដែលការសាកល្បងទាំងអស់ត្រូវការពេលយូរជាងអាយុសកលលោក — ធ្វើឱ្យ brute force មិនអាចធ្វើបាន។
- ហេតុនេះ **key វែង និងពាក្យសម្ងាត់ខ្លាំង** សំខាន់។

### 7) What are the differences between hashing and encryption? / តើភាពខុសគ្នារវាង hashing និង encryption ជាអ្វី?

| / | Hashing | Encryption |
|---|---|---|
| **Direction / ទិស** | One-way (irreversible) / មួយទិស (មិនអាចបញ្ច្រាស) | Two-way (reversible) / ពីរទិស (អាចបញ្ច្រាស) |
| **Key / សោ** | No key (or keyed for HMAC) / គ្មាន key (ឬមាន key សម្រាប់ HMAC) | Always uses a key / ប្រើ key ជានិច្ច |
| **Output / លទ្ធផល** | Fixed-length digest / digest ប្រវែងថេរ | Length related to input / ប្រវែងទាក់ទងនឹង input |
| **Goal / គោលដៅ** | Integrity, password storage / ភាពត្រឹមត្រូវ ការផ្ទុកពាក្យសម្ងាត់ | Confidentiality / ការសម្ងាត់ |
| **Get original back? / យកដើមវិញបាន?** | No — can't "un-hash" / ទេ — "un-hash" មិនបាន | Yes — decrypt with key / បាន — ឌិគ្រីបដោយ key |
| **Examples / ឧទាហរណ៍** | SHA-256, SHA-512, SHA-3 | AES, RSA, DES |

- **Key idea / គំនិតសំខាន់:** Encryption *protects secrecy* and can be undone with a key; hashing *verifies integrity* and is meant to be impossible to reverse. / Encryption *ការពារការសម្ងាត់* ហើយអាចត្រឡប់វិញដោយ key៖ hashing *ផ្ទៀងផ្ទាត់ភាពត្រឹមត្រូវ* ហើយមានន័យថាមិនអាចបញ្ច្រាស។

### 8) What is the difference between an "active attack" and a "passive attack"? / តើភាពខុសគ្នារវាង "active attack" និង "passive attack" ជាអ្វី?

**English:**
- **Passive attack:** the attacker only **observes or eavesdrops** without changing anything; the goal is to obtain information. Examples: sniffing/wiretapping, traffic analysis (studying patterns even if content is encrypted). Hard to detect (no trace) but prevented by encryption, which makes intercepted data unreadable.
- **Active attack:** the attacker **modifies, injects, deletes, replays, or fabricates** data, or disrupts service; the goal is to alter the system or impersonate. Examples: man-in-the-middle, message modification, masquerade/impersonation, replay attacks, denial-of-service. Can be detected (data changes) but harder to fully prevent; countered with authentication and integrity mechanisms (MACs, digital signatures).
- **Summary:** Passive = *listening only* (hard to detect, prevent with encryption); Active = *tampering/interfering* (detectable, defend with authentication and integrity checks).

**ខ្មែរ:**
- **Passive attack៖** អ្នកវាយប្រហារគ្រាន់តែ **សង្កេត ឬលួចស្ដាប់** ដោយមិនផ្លាស់ប្ដូរអ្វី៖ គោលដៅគឺទទួលព័ត៌មាន។ ឧទាហរណ៍៖ sniffing/wiretapping, traffic analysis (សិក្សាលំនាំ ទោះខ្លឹមសារត្រូវអ៊ិនគ្រីប)។ ពិបាករកឃើញ (គ្មានដាន) ប៉ុន្តែការពារដោយ encryption ដែលធ្វើឱ្យទិន្នន័យចាប់យកអានមិនបាន។
- **Active attack៖** អ្នកវាយប្រហារ **កែ បញ្ចូល លុប លេងឡើងវិញ (replay) ឬក្លែងបន្លំ** ទិន្នន័យ ឬរំខានសេវា៖ គោលដៅគឺផ្លាស់ប្ដូរប្រព័ន្ធ ឬក្លែងជា។ ឧទាហរណ៍៖ man-in-the-middle, ការកែសារ, masquerade/impersonation, replay attacks, denial-of-service។ អាចរកឃើញ (ទិន្នន័យផ្លាស់) ប៉ុន្តែពិបាកការពារពេញលេញ៖ ប្រឆាំងដោយយន្តការផ្ទៀងផ្ទាត់ និងភាពត្រឹមត្រូវ (MACs, ហត្ថលេខាឌីជីថល)។
- **សរុប៖** Passive = *ស្ដាប់តែប៉ុណ្ណោះ* (ពិបាករកឃើញ ការពារដោយ encryption)៖ Active = *កែ/រំខាន* (រកឃើញបាន ការពារដោយការផ្ទៀងផ្ទាត់ និងការត្រួតពិនិត្យភាពត្រឹមត្រូវ)។

### 9) Explain the difference between plaintext and ciphertext. / ពន្យល់ភាពខុសគ្នារវាង plaintext និង ciphertext។

**English:**
- **Plaintext** = the **original, readable** message or data *before* encryption — what you actually want to communicate (e.g. `HELLO`).
- **Ciphertext** = the **scrambled, unreadable** output produced *after* encrypting the plaintext (e.g. `KHOOR`). Without the correct key, it looks like meaningless data.
- Encryption turns plaintext into ciphertext; decryption turns ciphertext back into plaintext.

**ខ្មែរ:**
- **Plaintext** = សារ ឬទិន្នន័យ **ដើម អាចអានបាន** *មុន* ការអ៊ិនគ្រីប — អ្វីដែលអ្នកចង់ទំនាក់ទំនងពិតប្រាកដ (ឧ. `HELLO`)។
- **Ciphertext** = លទ្ធផល **ច្របូកច្របល់ អានមិនបាន** ដែលផលិត *ក្រោយ* ការអ៊ិនគ្រីប plaintext (ឧ. `KHOOR`)។ បើគ្មាន key ត្រឹមត្រូវ វាមើលទៅដូចទិន្នន័យគ្មានន័យ។
- Encryption បម្លែង plaintext ទៅ ciphertext៖ decryption បម្លែង ciphertext ត្រឡប់ទៅ plaintext។

### 10) What is a "cipher"? Give an example of a classical cipher. / តើ "cipher" ជាអ្វី? ផ្ដល់ឧទាហរណ៍នៃ classical cipher។

**English:**
- A **cipher** = an algorithm (a defined method) for performing encryption and decryption — the set of rules that transforms plaintext into ciphertext and back, controlled by a key.
- **Classical example — the Caesar cipher:** a *substitution* cipher that replaces each letter with one a fixed number of positions further along the alphabet. With a shift of 3: A→D, B→E, and `HELLO → KHOOR`.
- Other classical examples: the **Vigenère cipher** (using a keyword) and **transposition ciphers** (which rearrange the order of letters rather than substituting them).

**ខ្មែរ:**
- **Cipher** = algorithm (វិធីសាស្ត្រកំណត់) សម្រាប់ធ្វើការអ៊ិនគ្រីប និងឌិគ្រីប — សំណុំច្បាប់ដែលបម្លែង plaintext ទៅ ciphertext និងត្រឡប់វិញ គ្រប់គ្រងដោយ key។
- **ឧទាហរណ៍បុរាណ — Caesar cipher៖** cipher ប្រភេទ *ជំនួស (substitution)* ដែលជំនួសអក្សរនីមួយៗដោយអក្សរដែលនៅឆ្ងាយចំនួនថេរទៅមុខក្នុងអក្ខរក្រម។ ជាមួយការផ្លាស់ ៣៖ A→D, B→E ហើយ `HELLO → KHOOR`។
- ឧទាហរណ៍បុរាណផ្សេង៖ **Vigenère cipher** (ប្រើពាក្យគន្លឹះ) និង **transposition ciphers** (រៀបលំដាប់អក្សរឡើងវិញ ជំនួសការជំនួស)។

### 11) Why is it insecure to reuse the same password everywhere, and how does cryptography help? / ហេតុអ្វីការប្រើពាក្យសម្ងាត់ដូចគ្នាគ្រប់កន្លែងគ្មានសុវត្ថិភាព ហើយ cryptography ជួយយ៉ាងណា?

**English:**
- **Why it's insecure:** if you reuse one password and *any* single website is breached and its password database leaks, attackers take that password and try it on all your other accounts (email, banking, social media). This automated technique is **credential stuffing** — one breach then compromises *everything*. The weakest site you ever signed up to becomes the weak link for all your accounts.
- **How cryptography helps:**
  - **Hashing + salting** — reputable sites store **salted hashes**, not plaintext, so even if the database is stolen, the actual passwords are hard to recover.
  - **Password managers** — generate a unique, strong, random password for every account and store them in an encrypted vault; you remember only one master password.
  - **Multi-factor authentication and cryptographic tokens** — add a second layer so a stolen password alone is not enough.
- Together, cryptography protects stored passwords and makes it practical to use a different strong password for every account.

**ខ្មែរ:**
- **ហេតុអ្វីគ្មានសុវត្ថិភាព៖** បើអ្នកប្រើពាក្យសម្ងាត់តែមួយឡើងវិញ ហើយគេហទំព័រ *ណាមួយ* ត្រូវ breach ហើយ database ពាក្យសម្ងាត់លេចធ្លាយ អ្នកវាយប្រហារយកពាក្យសម្ងាត់នោះ ហើយសាកល្បងលើគណនីផ្សេងទាំងអស់របស់អ្នក (អ៊ីមែល ធនាគារ បណ្ដាញសង្គម)។ បច្ចេកទេសស្វ័យប្រវត្តិនេះហៅថា **credential stuffing** — breach មួយ បំផ្លាញ *អ្វីៗគ្រប់យ៉ាង*។ គេហទំព័រខ្សោយបំផុតដែលអ្នកធ្លាប់ចុះឈ្មោះ ក្លាយជាចំណុចខ្សោយសម្រាប់គណនីទាំងអស់។
- **Cryptography ជួយយ៉ាងណា៖**
  - **Hashing + salting** — គេហទំព័រល្បីៗផ្ទុក **salted hashes** មិនមែនអក្សរធម្មតា ដូច្នេះទោះ database ត្រូវលួច ពាក្យសម្ងាត់ពិតពិបាករកវិញ។
  - **Password managers** — បង្កើតពាក្យសម្ងាត់ប្លែក ខ្លាំង ចៃដន្យ សម្រាប់គណនីនីមួយៗ ហើយផ្ទុកក្នុង vault អ៊ិនគ្រីប៖ អ្នកចាំតែ master password មួយ។
  - **Multi-factor authentication និង cryptographic tokens** — បន្ថែមស្រទាប់ទីពីរ ដូច្នេះពាក្យសម្ងាត់ដែលត្រូវលួចតែម្នាក់ឯងមិនគ្រប់គ្រាន់។
- រួមគ្នា cryptography ការពារពាក្យសម្ងាត់ដែលផ្ទុក និងធ្វើឱ្យមានលទ្ធភាពប្រើពាក្យសម្ងាត់ខ្លាំងផ្សេងគ្នាសម្រាប់គណនីនីមួយៗ។

### 12) What is the main purpose of a "digital certificate" when you visit a secure (HTTPS) website? / តើគោលបំណងសំខាន់នៃ "digital certificate" ពេលអ្នកចូលគេហទំព័រសុវត្ថិភាព (HTTPS) ជាអ្វី?

**English:**
- A **digital certificate** (an X.509 certificate) is an electronic document, issued and signed by a trusted **Certificate Authority (CA)**, that binds a website's **identity** (its domain name) to its **public key**.
- **Main purposes on an HTTPS site:**
  - **Authentication / trust** — proves you're connecting to the genuine website and not an impostor, protecting against impersonation and man-in-the-middle attacks. Your browser checks the certificate was signed by a trusted CA and matches the site.
  - **Providing the public key** — supplies the site's public key, which your browser uses to securely establish an encrypted TLS session (typically exchanging a symmetric session key).
- In short, the certificate answers "is this site really who it claims to be?" and supplies the key needed to set up the encrypted connection (the padlock icon).

**ខ្មែរ:**
- **Digital certificate** (X.509 certificate) ជាឯកសារអេឡិចត្រូនិក ចេញ និងចុះហត្ថលេខាដោយ **Certificate Authority (CA)** ដែលជឿទុកចិត្ត ដែលភ្ជាប់ **អត្តសញ្ញាណ** គេហទំព័រ (ឈ្មោះ domain) ទៅ **public key** របស់វា។
- **គោលបំណងសំខាន់លើគេហទំព័រ HTTPS៖**
  - **ការផ្ទៀងផ្ទាត់ / ទំនុកចិត្ត** — បញ្ជាក់ថាអ្នកកំពុងភ្ជាប់ទៅគេហទំព័រពិត មិនមែនអ្នកក្លែងបន្លំ ការពារពី impersonation និង man-in-the-middle attacks។ browser ពិនិត្យថា certificate ត្រូវចុះហត្ថលេខាដោយ CA ជឿទុកចិត្ត និងត្រូវនឹងគេហទំព័រ។
  - **ផ្ដល់ public key** — ផ្ដល់ public key របស់គេហទំព័រ ដែល browser ប្រើដើម្បីបង្កើត TLS session អ៊ិនគ្រីបដោយសុវត្ថិភាព (ជាទូទៅផ្លាស់ប្ដូរ symmetric session key)។
- សរុប certificate ឆ្លើយថា "តើគេហទំព័រនេះពិតជាអ្នកដែលវាអះអាងឬ?" ហើយផ្ដល់ key ដែលត្រូវការ ដើម្បីបង្កើតការតភ្ជាប់អ៊ិនគ្រីប (រូបសោ)។

### 13) What is the main difference between symmetric and asymmetric encryption regarding how they use keys? / តើភាពខុសគ្នាសំខាន់រវាង symmetric និង asymmetric encryption ទាក់ទងនឹងរបៀបប្រើ key ជាអ្វី?

**English:**
- **Symmetric encryption** uses **one single shared secret key** for both encryption and decryption. Both sender and receiver must have the same key and keep it secret (e.g. AES).
- **Asymmetric encryption** uses a **pair of mathematically related keys** — a public key and a private key. One key encrypts and the *other* decrypts: typically the public key encrypts and only the matching private key decrypts. The public key can be shared openly; the private key is kept secret (e.g. RSA).
- **Main difference:** symmetric = one secret key shared by both parties; asymmetric = two keys per person (a public one and a private one), removing the need to share a secret key in advance.

**ខ្មែរ:**
- **Symmetric encryption** ប្រើ **secret key រួមតែមួយ** សម្រាប់ទាំងអ៊ិនគ្រីប និងឌិគ្រីប។ ទាំងអ្នកផ្ញើ និងអ្នកទទួល ត្រូវមាន key ដូចគ្នា និងរក្សាសម្ងាត់ (ឧ. AES)។
- **Asymmetric encryption** ប្រើ **គូ key ដែលទាក់ទងគ្នាតាមគណិតវិទ្យា** — public key និង private key។ key មួយអ៊ិនគ្រីប ហើយ *មួយទៀត* ឌិគ្រីប៖ ជាទូទៅ public key អ៊ិនគ្រីប ហើយតែ private key ដែលត្រូវគ្នាប៉ុណ្ណោះឌិគ្រីប។ public key អាចចែករំលែកជាសាធារណៈ៖ private key រក្សាសម្ងាត់ (ឧ. RSA)។
- **ភាពខុសគ្នាសំខាន់៖** symmetric = secret key តែមួយ ចែករំលែកដោយភាគីទាំងពីរ៖ asymmetric = key ពីរក្នុងម្នាក់ៗ (មួយសាធារណៈ មួយឯកជន) លុបតម្រូវការចែករំលែក secret key ជាមុន។

### 14) If Alice wants to send a secret message to Bob, which key should she use — Bob's public key or Bob's private key? Explain. / បើ Alice ចង់ផ្ញើសារសម្ងាត់ទៅ Bob តើនាងគួរប្រើ key ណា — public key ឬ private key របស់ Bob? ពន្យល់។

**English:**
- Alice should encrypt the message with **Bob's public key**.
- **Why:** in asymmetric cryptography, anything encrypted with Bob's public key can only be decrypted with Bob's private key — and Bob is the only one holding that private key. So only Bob can read the message, which guarantees confidentiality.
- She must **not** use Bob's private key — Alice doesn't have it (it's Bob's secret), and conceptually it wouldn't keep the message secret, because anything "locked" with a private key can be opened with the matching public key, which everyone knows. (Encrypting with a private key is what's done for digital signatures, not secrecy.) Using her own keys wouldn't work either, since Bob couldn't decrypt it.
- **Rule of thumb:** to send someone a secret, encrypt with the recipient's public key.

**ខ្មែរ:**
- Alice គួរអ៊ិនគ្រីបសារដោយ **public key របស់ Bob**។
- **ហេតុអ្វី៖** ក្នុង asymmetric cryptography អ្វីដែលអ៊ិនគ្រីបដោយ public key របស់ Bob អាចឌិគ្រីបបានតែដោយ private key របស់ Bob — ហើយ Bob ជាអ្នកតែម្នាក់កាន់ private key នោះ។ ដូច្នេះតែ Bob អាចអានសារ ដែលធានាការសម្ងាត់។
- នាង **មិនត្រូវ** ប្រើ private key របស់ Bob — Alice គ្មានវា (វាជាការសម្ងាត់របស់ Bob) ហើយតាមគំនិត វាក៏មិនរក្សាសារសម្ងាត់ដែរ ព្រោះអ្វីដែល "ចាក់សោ" ដោយ private key អាចបើកដោយ public key ដែលត្រូវគ្នា ដែលគ្រប់គ្នាដឹង។ (ការអ៊ិនគ្រីបដោយ private key គឺសម្រាប់ហត្ថលេខាឌីជីថល មិនមែនការសម្ងាត់។) ការប្រើ key ផ្ទាល់ខ្លួនរបស់នាងក៏មិនដំណើរការ ព្រោះ Bob ឌិគ្រីបមិនបាន។
- **ច្បាប់មេដៃ៖** ដើម្បីផ្ញើសារសម្ងាត់ទៅអ្នកណាម្នាក់ អ៊ិនគ្រីបដោយ public key របស់អ្នកទទួល។

### 15) What is "steganography," and how does it differ from traditional cryptography? / តើ "steganography" ជាអ្វី ហើយវាខុសពី cryptography បែបប្រពៃណីយ៉ាងណា?

**English:**
- **Steganography** = the practice of **hiding the very existence of a message** by concealing it inside ordinary-looking data — e.g. embedding secret text within the pixels of an image, an audio file, or a video — so an observer doesn't even realise a hidden message is present.

| / | Cryptography | Steganography |
|---|---|---|
| **What it hides / លាក់អ្វី** | The meaning/content of the message / អត្ថន័យ/ខ្លឹមសារ | The existence of the message / អត្ថិភាពនៃសារ |
| **Message visible? / សារមើលឃើញ?** | Yes, but as unreadable ciphertext / បាទ ប៉ុន្តែជា ciphertext អានមិនបាន | No — looks like an ordinary file / ទេ — មើលទៅដូចឯកសារធម្មតា |
| **Goal / គោលដៅ** | Make the message unreadable / ធ្វើឱ្យសារអានមិនបាន | Make the message undetectable / ធ្វើឱ្យសាររកមិនឃើញ |

- **In short:** cryptography scrambles a message so it cannot be *understood*; steganography hides a message so it cannot be *found*. A classic example is altering the least-significant bits of an image's pixels to embed hidden text invisibly. The two can be combined — encrypting a message *and then* hiding it — for even stronger protection.

**ខ្មែរ:**
- **Steganography** = ការអនុវត្ត **លាក់អត្ថិភាពនៃសារ** ដោយលាក់វាក្នុងទិន្នន័យដែលមើលទៅធម្មតា — ឧ. បង្កប់អក្សរសម្ងាត់ក្នុង pixels នៃរូបភាព ឯកសារសំឡេង ឬវីដេអូ — ដូច្នេះអ្នកសង្កេតមិនដឹងថាមានសារលាក់។

| / | Cryptography | Steganography |
|---|---|---|
| **លាក់អ្វី** | អត្ថន័យ/ខ្លឹមសារនៃសារ | អត្ថិភាពនៃសារ |
| **សារមើលឃើញ?** | បាទ ប៉ុន្តែជា ciphertext អានមិនបាន | ទេ — មើលទៅដូចឯកសារធម្មតា |
| **គោលដៅ** | ធ្វើឱ្យសារអានមិនបានចំពោះអ្នកក្រៅ | ធ្វើឱ្យសាររកមិនឃើញ |

- **សរុប៖** cryptography ច្របល់សារ ឱ្យ *យល់* មិនបាន៖ steganography លាក់សារ ឱ្យ *រក* មិនឃើញ។ ឧទាហរណ៍បុរាណគឺការផ្លាស់ប្ដូរ least-significant bits នៃ pixels រូបភាព ដើម្បីបង្កប់អក្សរលាក់ដោយមើលមិនឃើញ។ ទាំងពីរអាចបញ្ចូលគ្នា — អ៊ិនគ្រីបសារ *រួចបន្ទាប់មក* លាក់វា — សម្រាប់ការការពារកាន់តែខ្លាំង។
