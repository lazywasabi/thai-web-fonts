# เว็บฟอนต์ภาษาไทย

รวมเว็บฟอนต์ภาษาไทย สำหรับใช้งานผ่าน CDN

- ทุกฟอนต์สามารถใช้งานเชิงพาณิชย์ได้ ดูสัญญาอนุญาตได้ในรายชื่อฟอนต์ด้านล่าง
- รองรับเฉพาะไฟล์ชนิด woff2 (ไฟล์ woff ใช้งานได้ในเวอร์ชัน [2.0.0](https://github.com/lazywasabi/thai-web-fonts/tree/v2.0.0))

## การใช้งาน

### ดาวน์โหลด

ดาวน์โหลดไฟล์เวอร์ชันล่าสุดได้ที่ทาง [GitHub Releases](https://github.com/lazywasabi/thai-web-fonts/releases)

### ใช้งานผ่าน CDN

ใช้ [jsDelivr](https://www.jsdelivr.com/) เพื่อใช้งานฟอนต์ผ่าน CDN

```
https://cdn.jsdelivr.net/gh/lazywasabi/thai-web-fonts@3/fonts/ชื่อฟอนต์/ชื่อไฟล์.woff2
```

ดูรายชื่อไฟล์ที่ใช้งานได้ พร้อมลิงก์ CDN ได้[ที่นี่](https://cdn.jsdelivr.net/gh/lazywasabi/thai-web-fonts@3/fonts/)

ตัวอย่างการใช้งาน:

```css
@font-face {
  font-family: 'Noto Sans Thai';
  src: url('https://cdn.jsdelivr.net/gh/lazywasabi/thai-web-fonts@3/fonts/NotoSansThai/NotoSansThai-Regular.woff2')
    format('woff2');
  font-style: normal;
  font-weight: normal;
  font-display: swap;
}

@font-face {
  font-family: 'Noto Sans Thai';
  src: url('https://cdn.jsdelivr.net/gh/lazywasabi/thai-web-fonts@3/fonts/NotoSansThai/NotoSansThai-Bold.woff2')
    format('woff2');
  font-style: normal;
  font-weight: bold;
  font-display: swap;
}
```

### การกำหนดเลขเวอร์ชัน

ผมไม่แนะนำให้ลบเลขเวอร์ชันออกจาก URL หรือใช้ `@latest` เพราะในกรณีที่มีการเปลี่ยนแปลงรูปแบบไฟล์ URL เดิมจะยังคงสามารถใช้งานได้ตามปกติ

โดยการกำหนดเลขเวอร์ชันผมจะใช้ระบบคล้าย [semver](https://semver.org/)

- หลักแรก (Major): จะปรับเมื่อมีการเปลี่ยนแปลงไฟล์ที่ส่งผลต่อ URL เช่นจาก [เวอร์ชัน 2.0.0 เป็น 3.0.0](https://github.com/lazywasabi/thai-web-fonts/compare/v2.0.0...v3.0.0) เนื่องจากมีการลบไฟล์ woff
- หลักที่สอง (Minor): จะปรับเมื่อมีการเปลี่ยนแปลงไฟล์ที่ไม่ส่งผลต่อ URL แต่อาจส่งผลต่อการแสดงผลฟอนต์ เช่น เพิ่มฟอนต์ใหม่ หรืออัปเดตเวอร์ชันฟอนต์
- หลักที่สาม (Patch): จะปรับเมื่อมีการเปลี่ยนแปลงที่ไม่ส่งผลต่อ URL และการแสดงผลฟอนต์

สำหรับการใช้งานทั่วไป ผมแนะนำให้ใช้เลขเวอร์ชันหลักแรกอย่างเดียวได้เลยครับ (แบบในตัวอย่างด้านบน) เพราะจะได้ใช้ฟอนต์เวอร์ชันล่าสุด และไม่ส่งผลต่อ URL ไฟล์

สามารถดูวิธีกำหนดเวอร์ชันใน URL เพิ่มเติมได้ที่[เว็บไซต์ของ jsDelivr](https://www.jsdelivr.com/features#gh) และ[ดูบันทึกการเปลี่ยนแปลงได้บน GitHub](https://github.com/lazywasabi/thai-web-fonts/releases)

## รายชื่อฟอนต์

### [Anakotmai](fonts/Anakotmai)

เว็บไซต์: https://futureforwardparty.org/?page_id=1242  
สัญญาอนุญาต: [Public Domain](https://futureforwardparty.org/?page_id=1242)

### [Anuphan](fonts/Anuphan)

เว็บไซต์: https://www.cadsondemak.com/medias/read/design-like-a-bilingual-ibm-plex-thai  
ซอร์สโค้ด: https://github.com/cadsondemak/Anuphan  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/cadsondemak/Anuphan/blob/master/OFL.txt)

### [Athiti](fonts/Athiti)

เว็บไซต์: https://cadsondemak.github.io/athiti/  
ซอร์สโค้ด: https://github.com/cadsondemak/athiti  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/cadsondemak/athiti/blob/master/OFL)

### [Bai Jamjuree](fonts/BaiJamjuree)

เว็บไซต์: https://cadsondemak.github.io/Bai-Jamjuree/  
ซอร์สโค้ด: https://github.com/cadsondemak/Bai-Jamjuree  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/cadsondemak/Bai-Jamjuree/blob/master/OFL.txt)

### [Chakra Petch](fonts/ChakraPetch)

เว็บไซต์: https://cadsondemak.github.io/chakra-petch/  
ซอร์สโค้ด: https://github.com/cadsondemak/Chakra-Petch  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/cadsondemak/Chakra-Petch/blob/master/OFL.txt)

### [Charm](fonts/Charm)

เว็บไซต์: https://cadsondemak.github.io/Charm/  
ซอร์สโค้ด: https://github.com/cadsondemak/Charm  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/cadsondemak/Charm/blob/master/OFL.txt)

### [Charmonman](fonts/Charmonman)

เว็บไซต์: https://cadsondemak.github.io/Charmonman/  
ซอร์สโค้ด: https://github.com/cadsondemak/Charmonman  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/cadsondemak/Charmonman/blob/master/OFL.txt)

### [Chonburi](fonts/Chonburi)

เว็บไซต์: https://cadsondemak.github.io/chonburi/  
ซอร์สโค้ด: https://github.com/cadsondemak/chonburi  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/cadsondemak/chonburi/blob/master/OFL.txt)

### [Chulabhorn Likit](fonts/ChulabhornLikit)

เว็บไซต์: https://www.cra.ac.th/th/download_fonts  
สัญญาอนุญาต: SIL Open Font License, version 1.1 (อ้างอิงจาก[คัดสรร ดีมาก](https://www.cadsondemak.com/medias/read/cra-point-of-view))

### [Droid Sans Thai](fonts/DroidSansThai)

สัญญาอนุญาต: [Apache License, version 2.0](https://fonts.gstatic.com/ea/droidsansthai/v4/LICENSE.txt)

### [Fahkwang](fonts/Fahkwang)

เว็บไซต์: https://cadsondemak.github.io/Fah-Kwang/  
ซอร์สโค้ด: https://github.com/cadsondemak/Fah-Kwang  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/cadsondemak/Fah-Kwang/blob/master/OFL.txt)

### [Garuda](fonts/Garuda)

เว็บไซต์: https://linux.thai.net/projects/fonts-tlwg  
ซอร์สโค้ด: https://github.com/tlwg/fonts-tlwg  
สัญญาอนุญาต: [GNU General Public License, version 2](https://github.com/tlwg/fonts-tlwg/blob/master/COPYING)

### [IBM Plex Sans Thai](fonts/IBMPlexSansThai)

เว็บไซต์: https://www.ibm.com/plex/  
ซอร์สโค้ด: https://github.com/IBM/plex  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/IBM/plex/blob/master/LICENSE.txt)

### [IBM Plex Sans Thai Looped](fonts/IBMPlexSansThaiLooped)

เว็บไซต์: https://www.ibm.com/plex/  
ซอร์สโค้ด: https://github.com/IBM/plex  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/IBM/plex/blob/master/LICENSE.txt)

### [Itim](fonts/Itim)

เว็บไซต์: https://cadsondemak.github.io/itim/  
ซอร์สโค้ด: https://github.com/cadsondemak/itim  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/cadsondemak/itim/blob/master/OFL.txt)

### [K2D](fonts/K2D)

เว็บไซต์: https://cadsondemak.github.io/K2D/  
ซอร์สโค้ด: https://github.com/cadsondemak/K2D  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/cadsondemak/K2D/blob/master/OFL.txt)

### [Kanit](fonts/Kanit)

เว็บไซต์: https://cadsondemak.github.io/kanit/  
ซอร์สโค้ด: https://github.com/cadsondemak/kanit  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/cadsondemak/kanit/blob/master/OFL.txt)

### [Kinnari](fonts/Kinnari)

เว็บไซต์: https://linux.thai.net/projects/fonts-tlwg  
ซอร์สโค้ด: https://github.com/tlwg/fonts-tlwg  
สัญญาอนุญาต: [GNU General Public License, version 2](https://github.com/tlwg/fonts-tlwg/blob/master/COPYING)

### [Kodchasan](fonts/Kodchasan)

เว็บไซต์: https://cadsondemak.github.io/Kodchasan/  
ซอร์สโค้ด: https://github.com/cadsondemak/Kodchasan  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/cadsondemak/Kodchasan/blob/master/OFL.txt)

### [Koho](fonts/Koho)

เว็บไซต์: https://cadsondemak.github.io/Koho/  
ซอร์สโค้ด: https://github.com/cadsondemak/Koho  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/cadsondemak/Koho/blob/master/OFL.txt)

### [Krub](fonts/Krub)

เว็บไซต์: https://cadsondemak.github.io/Krub/  
ซอร์สโค้ด: https://github.com/cadsondemak/Krub  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/cadsondemak/Krub/blob/master/OFL.txt)

### [Loma](fonts/Loma)

เว็บไซต์: https://linux.thai.net/projects/fonts-tlwg  
ซอร์สโค้ด: https://github.com/tlwg/fonts-tlwg  
สัญญาอนุญาต: [GNU General Public License, version 2](https://github.com/tlwg/fonts-tlwg/blob/master/COPYING)

### [Maitree](fonts/Maitree)

เว็บไซต์: https://cadsondemak.github.io/maitree/  
ซอร์สโค้ด: https://github.com/cadsondemak/maitree  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/cadsondemak/maitree/blob/master/OFL.txt)

### [Mali](fonts/Mali)

เว็บไซต์: https://cadsondemak.github.io/mitr/  
ซอร์สโค้ด: https://github.com/cadsondemak/mitr  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/cadsondemak/mitr/blob/master/OFL)

### [Mitr](fonts/Mitr)

เว็บไซต์: https://cadsondemak.github.io/Mali/  
ซอร์สโค้ด: https://github.com/cadsondemak/Mali  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/cadsondemak/Mali/blob/master/OFL.txt)

### [Niramit](fonts/Niramit)

เว็บไซต์: https://cadsondemak.github.io/Niramit/  
ซอร์สโค้ด: https://github.com/cadsondemak/Niramit  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/cadsondemak/Niramit/blob/master/OFL.txt)

### [Noto Sans Thai](fonts/NotoSansThai)

เว็บไซต์: https://fonts.google.com/noto/specimen/Noto+Sans+Thai  
ซอร์สโค้ด: https://github.com/googlefonts/noto-fonts  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/googlefonts/noto-fonts/blob/main/LICENSE)

### [Noto Sans Thai Looped](fonts/NotoSansThaiLooped)

**หมายเหตุ:** build จากซอร์สบน GitHub [ดูรายละเอียดเพิ่มเติม](https://lazywasabi.com/blog/noto-sans-thai-looped/)  
เว็บไซต์: https://fonts.google.com/noto/specimen/Noto+Sans+Thai+Looped  
ซอร์สโค้ด: https://github.com/googlefonts/noto-fonts  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/googlefonts/noto-fonts/blob/main/LICENSE)

### [Noto Serif Thai](fonts/NotoSerifThai)

เว็บไซต์: https://fonts.google.com/noto/specimen/Noto+Serif+Thai  
ซอร์สโค้ด: https://github.com/googlefonts/noto-fonts  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/googlefonts/noto-fonts/blob/main/LICENSE)

### [Pattaya](fonts/Pattaya)

เว็บไซต์: https://cadsondemak.github.io/pattaya/  
ซอร์สโค้ด: https://github.com/cadsondemak/pattaya  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/cadsondemak/pattaya/blob/master/OFL.txt)

### [Pridi](fonts/Pridi)

เว็บไซต์: https://cadsondemak.github.io/pridi/  
ซอร์สโค้ด: https://github.com/cadsondemak/pridi  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/cadsondemak/pridi/blob/master/OFL)

### [Prompt](fonts/Prompt)

เว็บไซต์: https://cadsondemak.github.io/prompt/  
ซอร์สโค้ด: https://github.com/cadsondemak/prompt  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/cadsondemak/prompt/blob/master/OFL.txt)

### [Sarabun](fonts/Sarabun)

เว็บไซต์: https://cadsondemak.github.io/Sarabun/  
ซอร์สโค้ด: https://github.com/cadsondemak/sarabun  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/cadsondemak/Sarabun/blob/master/OFL.txt)

### [Srisakdi](fonts/Srisakdi)

เว็บไซต์: https://cadsondemak.github.io/Srisakdi/  
ซอร์สโค้ด: https://github.com/cadsondemak/Srisakdi  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/cadsondemak/Srisakdi/blob/master/OFL.txt)

### [Sriracha](fonts/Sriracha)

เว็บไซต์: https://cadsondemak.github.io/sriracha/  
ซอร์สโค้ด: https://github.com/cadsondemak/sriracha  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/cadsondemak/sriracha/blob/master/OFL.txt)

### [Taviraj](fonts/Taviraj)

เว็บไซต์: https://cadsondemak.github.io/taviraj/  
ซอร์สโค้ด: https://github.com/cadsondemak/taviraj  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/cadsondemak/taviraj/blob/master/OFL.txt)

### [Thasadith](fonts/Thasadith)

เว็บไซต์: https://cadsondemak.github.io/Thasadith/  
ซอร์สโค้ด: https://github.com/cadsondemak/Thasadith  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/cadsondemak/Thasadith/blob/master/OFL.txt)

### [TlwgTypewriter](fonts/TlwgTypewriter)

เว็บไซต์: https://linux.thai.net/projects/fonts-tlwg  
ซอร์สโค้ด: https://github.com/tlwg/fonts-tlwg  
สัญญาอนุญาต: [GNU General Public License, version 2](https://github.com/tlwg/fonts-tlwg/blob/master/COPYING)

### [TlwgTypist](fonts/TlwgTypist)

เว็บไซต์: https://linux.thai.net/projects/fonts-tlwg  
ซอร์สโค้ด: https://github.com/tlwg/fonts-tlwg  
สัญญาอนุญาต: [GNU General Public License, version 2](https://github.com/tlwg/fonts-tlwg/blob/master/COPYING)

### [Trirong](fonts/Trirong)

เว็บไซต์: https://cadsondemak.github.io/trirong/  
ซอร์สโค้ด: https://github.com/cadsondemak/trirong  
สัญญาอนุญาต: [SIL Open Font License, version 1.1](https://github.com/cadsondemak/trirong/blob/master/OFL.txt)

### [Umpush](fonts/Umpush)

เว็บไซต์: https://linux.thai.net/projects/fonts-tlwg  
ซอร์สโค้ด: https://github.com/tlwg/fonts-tlwg  
สัญญาอนุญาต: [GNU General Public License, version 2](https://github.com/tlwg/fonts-tlwg/blob/master/COPYING)
