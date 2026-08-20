---
tags:
  - computer-science
  - advance
  - data-representation
  - ipst
source: "IPST (สสวท.) Computer Science Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว331"]
---

# Data Representation — การเก็บข้อมูลในคอมพิวเตอร์

> *"All information is reducible to a sequence of bits — ones and zeros, yes and no."* — adapted from Claude Shannon

Computers store and process all data — numbers, text, images, and sound — as binary (เลขฐานสอง), sequences of 0s and 1s called bits (บิต). The IPST curriculum for ม.4 (ว331) covers how different types of real-world information are encoded into binary so the computer can manipulate them.

Understanding data representation (การเก็บข้อมูล) reveals the bridge between the analogue human world and the digital machine world. Students learn number-system conversions, character encoding schemes (ASCII, Unicode), and how multimedia (images, sound) is discretised, compressed, and stored.

---

## 1 | Course Coverage

### ม.4 (ว331)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Binary number system; conversions between binary, decimal, hexadecimal; bits and bytes | Convert between bases, explain bit/byte units |
| **Semester 2** | ASCII and Unicode; image (bitmap, RGB) and sound representation; data compression (lossy/lossless) | Encode text, calculate file sizes, distinguish compression types |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| เลขฐานสอง | Binary | Base 2 (0,1) |
| เลขฐานสิบ | Decimal | Base 10 (0–9) |
| เลขฐานสิบหก | Hexadecimal | Base 16 (0–9,A–F) |
| บิต | Bit | 0 or 1 |
| ไบต์ | Byte | 8 bits |
| รหัสอักขระ | Character Encoding | ASCII / Unicode |
| พิกเซล | Pixel | Picture element |
| ความละเอียด | Resolution | pixels per inch |
| อัตราตัวอย่าง | Sampling Rate | Hz |
| ความลึกบิต | Bit Depth | bits per sample |
| การบีบอัดข้อมูล | Data Compression | lossy / lossless |

---

## 3 | Key Concepts

### 3.1 Number Systems (ระบบเลข)

Computers use binary (เลขฐานสอง) because electronic components have two stable states (on/off). Humans use decimal (เลขฐานสิบ); programmers also use hexadecimal (เลขฐานสิบหก) as a compact binary shorthand.

| System | Base | Digits | Example |
|---|---|---|---|
| Decimal | 10 | 0–9 | $25_{10}$ |
| Binary | 2 | 0, 1 | $11001_2$ |
| Hexadecimal | 16 | 0–9, A–F | $19_{16}$ |

**Decimal → Binary:** repeatedly divide by 2, read remainders bottom-up.

$$25 \div 2 = 12 \text{ r } 1 \;\Rightarrow\; 25_{10} = 11001_2$$

**Binary → Decimal:** multiply each bit by its place value.

$$11001_2 = 16 + 8 + 0 + 0 + 1 = 25_{10}$$

**Binary ↔ Hexadecimal:** group bits in fours from the right.

$$1100\,1100_2 = \text{CC}_{16}$$

### 3.2 Bits, Bytes, and Units

- **Bit (บิต):** smallest unit, value 0 or 1.
- **Byte (ไบต์):** 8 bits.
- Larger units: KB = $2^{10}$ bytes, MB = $2^{20}$ bytes, GB = $2^{30}$ bytes, TB = $2^{40}$ bytes.

### 3.3 Character Encoding (รหัสอักขระ)

**ASCII** uses 7 bits → 128 characters (English letters, digits, punctuation). Each character maps to a number: `'A'` = 65, `'a'` = 97, `'0'` = 48.

**Unicode (ยูนิโค้ด)** extends ASCII to cover all world scripts. UTF-8 uses 1–4 bytes per character; it can represent Thai, Chinese, Arabic, emoji, etc. The Thai block starts at U+0E01.

### 3.4 Image Representation (การเก็บภาพ)

A **bitmap image (ภาพบิตแมป)** is a grid of pixels (พิกเซล). Each pixel stores colour information.

- **Black & white:** 1 bit per pixel (0 = black, 1 = white).
- **Grayscale:** 8 bits per pixel → 256 grey levels.
- **Colour (RGB):** 3 channels (Red, Green, Blue), 8 bits each → 24-bit colour, $2^{24} \approx 16.7$ million colours.

**File size formula:**

$$\text{Size (bytes)} = \text{width} \times \text{height} \times \text{bits per pixel} \div 8$$

**Resolution (ความละเอียด)** — more pixels → sharper image but larger file.

### 3.5 Sound Representation (การเก็บเสียง)

Sound is an analogue (อนาล็อก) wave; computers sample it at regular intervals:

- **Sampling rate (อัตราตัวอย่าง):** samples per second (Hz). CD quality = 44 100 Hz.
- **Bit depth (ความลึกบิต):** bits per sample (16-bit is standard).

$$\text{Size (bytes)} = \text{sampling rate} \times \text{bit depth} \div 8 \times \text{channels} \times \text{duration (s)}$$

### 3.6 Data Compression (การบีบอัดข้อมูล)

| Type | Description | Example |
|---|---|---|
| **Lossless (ไม่สูญเสีย)** | Reconstructs exact original data | PNG, FLAC, ZIP |
| **Lossy (สูญเสียบางส่วน)** | Discards less-noticeable detail for smaller size | JPEG, MP3, MP4 |

---

## 4 | Common Problem Types

### Type 1: Base Conversion
> Convert $45_{10}$ to binary and hexadecimal.

**Solution:**

```python
n = 45
print(bin(n))   # 0b101101
print(hex(n))   # 0x2d
```

$45_{10} = 101101_2 = \text{2D}_{16}$.

### Type 2: Image File Size
> A 1024×768 RGB (24-bit) image is stored uncompressed. Calculate its size in MB.

**Solution:**

$$1024 \times 768 \times 24 \div 8 = 2\,359\,296 \text{ bytes} \approx 2.25 \text{ MB}$$

```python
size_bytes = 1024 * 768 * 24 // 8
print(size_bytes / (1024**2), "MB")  # 2.25 MB
```

### Type 3: Encoding Length
> How many bytes does the UTF-8 string "สวัสดี" occupy?

**Solution:** Thai characters use 3 bytes each in UTF-8; "สวัสดี" has 6 characters → $6 \times 3 = 18$ bytes.

```python
s = "สวัสดี"
print(len(s.encode("utf-8")))   # 18
```

---

## 5 | Cross-Links

- [[01_Computational_Thinking]] — abstraction applied to data
- [[03_Boolean_Logic]] — binary values as logical true/false
- [[06_Algorithms]] — algorithms operate on binary data
- [[01_Numbers_and_Numeration|Mathematics: Number Systems]] — base conversion foundations
