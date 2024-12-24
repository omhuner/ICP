--ENG-- 
(Turkish text is below )
# PhoneBook Actor

   Hello! My name is Ömer Hüner. I am 25 years old and a recent graduate of Anadolu University's English Business Administration program. 
I am currently learning data analysis and aim to pursue a career in this field. I am participating in various bootcamps and internships to improve myself. 
This project was developed during a Web3-focused workshop as part of an internship at Patika.dev. Its purpose is to create a phonebook application and implement basic data and message management functionalities.

## Features

- **Add Contact:** Add a contact to the phonebook with a name, phone number, and description.
- **Send Message:** Send a message and save it in the message history.
- **Retrieve Contact Information:** Retrieve contact details by name.
- **Retrieve Message History:** Access message history by phone number.

## Usage

1. **Add Contact**
   ```motoko
   await actor.insert("John Doe", {desc = "Friend", phone = "123-456-7890"});
   ```

2. **Send Message**
   ```motoko
   await actor.sendMessage("123-456-7890", {receiver = "John Doe", mess = "Hello!"});
   ```

3. **Retrieve Contact Information**
   ```motoko
   let contact = await actor.getPhone("John Doe");
   ```


4. **Retrieve Message History**
   ```motoko
   let message = await actor.getMessage("123-456-7890");
   ```


--TÜRKÇE--
# Telefon Rehberi

Merhaba! Ben Ömer Hüner. 25 yaşındayım ve Anadolu Üniversitesi İngilizce İşletme bölümünden yeni mezun oldum. 
Şu anda veri analizi öğreniyorum ve kariyerime bu alanda devam etmek istiyorum. Çeşitli bootcamp'lere ve stajlara katılarak kendimi geliştirmeye çalışıyorum. 
Bu proje, Patika.dev'deki bir staj sırasında yapılan Web3 odaklı bir workshopta geliştirilmiştir. Amacı, bir telefon rehberi uygulaması oluşturarak, temel veri ve mesaj yönetimi özelliklerini uygulamaktır.

## Özellikler

- **Kişi Ekleme:** Telefon rehberine bir isim, telefon numarası ve açıklama ile kişi ekleme.
- **Mesaj Gönderme:** Mesaj gönderme ve mesaj geçmişini kaydetme.
- **Kişi Bilgisi Alma:** İsme göre kişi bilgilerini getirme.
- **Mesaj Geçmişi Alma:** Telefon numarasına göre mesaj geçmişine erişim.

## Kullanım

1. **Kişi Ekleme**
   ```motoko
   await actor.insert("John Doe", {desc = "Arkadaş", phone = "123-456-7890"});
   ```

2. **Mesaj Gönderme**
   ```motoko
   await actor.sendMessage("123-456-7890", {receiver = "John Doe", mess = "Merhaba!"});
   ```

3. **Kişi Bilgisi Alma**
   ```motoko
   let contact = await actor.getPhone("John Doe");
   ```

4. **Mesaj Geçmişi Alma**
   ```motoko
   let message = await actor.getMessage("123-456-7890");
   ```
