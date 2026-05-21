import { useState, useEffect, useCallback } from "react";

const ALL_QUESTIONS = [
  { id: 1, q: "Geodeziya so'zi yunonchadan qanday ma'noni anglatadi?", correct: "Yer o'lchash va yer bo'lish", options: ["Yer o'lchash va yer bo'lish", "Yer shakli va tuzilishi", "Xarita chizish san'ati", "Yerning aylanishi"] },
  { id: 2, q: "Yerning shakli va o'lchamlarini aniqlash bilan shug'ullanuvchi fan nima?", correct: "Geodeziya", options: ["Geodeziya", "Kartografiya", "Topografiya", "Astronomiya"] },
  { id: 3, q: "Butun Yer sirtini yoki uning katta qismlarini shaklini o'rganuvchi soha qaysi?", correct: "Oliy geodeziya", options: ["Oliy geodeziya", "Injenerlik geodeziyasi", "Topografiya", "Fototopografiya"] },
  { id: 4, q: "Yer sirtining katta bo'lmagan bo'laklarining planlarini tuzish bilan nima shug'ullanadi?", correct: "Geodeziya yoki topografiya", options: ["Geodeziya yoki topografiya", "Oliy geodeziya", "Kartografiya", "Kosmik geodeziya"] },
  { id: 5, q: "Injenerlik inshootlarini qidiruv va loyihalashda qaysi geodeziya turi qo'llaniladi?", correct: "Injenerlik geodeziyasi", options: ["Injenerlik geodeziyasi", "Oliy geodeziya", "Kosmik geodeziya", "Fototopografiya"] },
  { id: 6, q: "Yer sirtini suratga olish va aerosuratlar orqali xarita tuzish nima deb ataladi?", correct: "Fototopografiya", options: ["Fototopografiya", "Kartografiya", "Kosmik geodeziya", "Topografiya"] },
  { id: 7, q: "Xaritalarni tuzish, nashr qilish va ulardan foydalanish usullarini o'rganuvchi fan qaysi?", correct: "Kartografiya", options: ["Kartografiya", "Geodeziya", "Topografiya", "Geoinformatika"] },
  { id: 8, q: "Yerning sun'iy yo'ldoshidan turib uning shaklini aniqlash nima deb ataladi?", correct: "Kosmik geodeziya", options: ["Kosmik geodeziya", "Oliy geodeziya", "Fototopografiya", "GNSS o'lchash"] },
  { id: 9, q: "Balandlik farqlarini aniqlashda ishlatiladigan asosiy geodezik asbob qaysi?", correct: "Niveller", options: ["Niveller", "Teodolit", "Total stansiya", "Bussol"] },
  { id: 10, q: "Gorizontal va vertikal burchaklarni o'lchash uchun qaysi asbob qo'llaniladi?", correct: "Teodolit", options: ["Teodolit", "Niveller", "Total stansiya", "GNSS qabul qilgich"] },
  { id: 11, q: "Masofa, burchak va balandlikni bir vaqtda o'lchovchi zamonaviy asbob nima?", correct: "Total stansiya", options: ["Total stansiya", "Teodolit", "Niveller", "Elektron ruletka"] },
  { id: 12, q: "Global navigatsion sun'iy yo'ldosh tizimining qisqartma nomi qanday?", correct: "GNSS", options: ["GNSS", "GPS", "GLONASS", "GIS"] },
  { id: 13, q: "Abu Rayhon Beruniy hisobi bo'yicha Yer radiusi qancha deb topilgan?", correct: "6339,58 km", options: ["6339,58 km", "6371,11 km", "6400 km", "6350 km"] },
  { id: 14, q: "Hozirgi vaqtda ishlatilayotgan Krasovskiy ellipsoidi radiusi qanchaga teng?", correct: "6371,11 km", options: ["6371,11 km", "6339,58 km", "6356 km", "6378 km"] },
  { id: 15, q: "Yer yuzasidagi eng baland nuqta bo'lgan Everest cho'qqisining balandligi qancha?", correct: "8848 m", options: ["8848 m", "8611 m", "7495 m", "9000 m"] },
  { id: 16, q: "Tinch okeanidagi eng chuqur nuqta bo'lgan Marian novisining chuqurligi qancha?", correct: "11022 m", options: ["11022 m", "10000 m", "9500 m", "12000 m"] },
  { id: 17, q: "Yer yuzasining necha foizini suv (okean va dengizlar) tashkil qiladi?", correct: "71 foiz", options: ["71 foiz", "60 foiz", "75 foiz", "65 foiz"] },
  { id: 18, q: "Yer yuzasining necha foizini quruqlik qismi tashkil qiladi?", correct: "29 foiz", options: ["29 foiz", "40 foiz", "25 foiz", "35 foiz"] },
  { id: 19, q: "1873-yilda Yerning haqiqiy shaklini geoid deb atagan olim kim?", correct: "Listing", options: ["Listing", "Beruniy", "Eratosfen", "Pifagor"] },
  { id: 20, q: "Yer yuzasidagi quruqliklarning o'rtacha balandligi dengiz sathidan qancha?", correct: "875 m", options: ["875 m", "500 m", "1000 m", "750 m"] },
  { id: 21, q: "Yer sharining o'lchamlarini aniqlagan va maxsus kitob yozgan yunon olimi kim?", correct: "Eratosfen", options: ["Eratosfen", "Pifagor", "Arximed", "Ptolomey"] },
  { id: 22, q: "Miloddan 6 asr ilgari Yerni shar shaklida deb aytgan olim qaysi?", correct: "Pifagor", options: ["Pifagor", "Eratosfen", "Aristotel", "Platon"] },
  { id: 23, q: "Algebra fanining asoschisi va 'Yer surati' asari muallifi kim?", correct: "Al-Xorazmiy", options: ["Al-Xorazmiy", "Beruniy", "Ibn Sino", "Al-Farg'oniy"] },
  { id: 24, q: "Beruniy yozgan 150 ta asaridan nechtasi geodeziya faniga bag'ishlangan?", correct: "40 tasi", options: ["40 tasi", "20 tasi", "50 tasi", "30 tasi"] },
  { id: 25, q: "O'lchov natijalarini qayd qilishda asosan nimalardan foydalaniladi?", correct: "Maxsus daftar yoki jadval", options: ["Maxsus daftar yoki jadval", "Oddiy daftar", "Kompyuter", "Telefon"] },
  { id: 26, q: "Teodolit yoki total stansiyani stativga o'rnatishda nima muhim hisoblanadi?", correct: "Asbobni to'g'ri o'rnatish va sozlash", options: ["Asbobni to'g'ri o'rnatish va sozlash", "Tezda ishga tushirish", "Batareyani zaryadlash", "Nur yo'nalishini tanlash"] },
  { id: 27, q: "Niveller bilan birgalikda balandliklarni o'qish uchun nima ishlatiladi?", correct: "Reyka", options: ["Reyka", "Stativ", "Bussol", "Ruletka"] },
  { id: 28, q: "Bino relyefining tikligini va qiyalik burchaklarini qaysi burchaklar orqali o'lchanadi?", correct: "Vertikal burchaklar", options: ["Vertikal burchaklar", "Gorizontal burchaklar", "Azimut burchaklari", "Magnit burchaklar"] },
  { id: 29, q: "Masofani o'lchashning eng qadimiy va oddiy usuli qaysi?", correct: "Ruletka yoki o'lchov lenta", options: ["Ruletka yoki o'lchov lenta", "Total stansiya", "GNSS", "Lazer o'lchagich"] },
  { id: 30, q: "Dron yordamida s'yomka qilishning asosiy afzalligi nimada?", correct: "Tezkor va keng qamrovli s'yomka", options: ["Tezkor va keng qamrovli s'yomka", "Arzon narx", "Yuqori aniqlik", "Suv ostini o'lchash"] },
  { id: 31, q: "Geoinformatika ma'lumotlarini tahlil qilishda qaysi dastur keng qo'llaniladi?", correct: "ArcGIS", options: ["ArcGIS", "AutoCAD", "MS Excel", "MATLAB"] },
  { id: 32, q: "MDH mamlakatlarida mutlaq balandliklar qaysi dengiz sathidan boshlanadi?", correct: "Boltiq dengizi sathidan", options: ["Boltiq dengizi sathidan", "Qora dengiz sathidan", "Kaspiy dengizi sathidan", "Orol dengizi sathidan"] },
  { id: 33, q: "Kronshtadt futshtoki nima maqsad uchun o'rnatilgan?", correct: "Dengiz sathini aniqlash uchun", options: ["Dengiz sathini aniqlash uchun", "Kema harakatini nazorat qilish uchun", "Geodezik nuqta uchun", "Meteorologik o'lchov uchun"] },
  { id: 34, q: "Plan va xaritalarda joyning haqiqiy holatini aks ettira olmasligi nima deyiladi?", correct: "Eskirish", options: ["Eskirish", "Buzilish", "Xato", "Deformatsiya"] },
  { id: 35, q: "Plan-kartografik materiallarning eskirishiga sabab bo'luvchi tabiiy omil qaysi?", correct: "Eroziya", options: ["Eroziya", "Zilzila", "Suv toshqini", "Yong'in"] },
  { id: 36, q: "Yer yuzasidagi nuqtani ekvatordan shimol yoki janubda ekanligini nima ko'rsatadi?", correct: "Geografik kenglik", options: ["Geografik kenglik", "Geografik uzunlik", "Magnit azimut", "Geodezik koordinata"] },
  { id: 37, q: "Boshlang'ich meridian sifatida qaysi shahar yaqinidagi observatoriya qabul qilingan?", correct: "Grinvich observatoriyasi", options: ["Grinvich observatoriyasi", "Parij observatoriyasi", "Berlin observatoriyasi", "London observatoriyasi"] },
  { id: 38, q: "Ekvatorda joylashgan nuqtalarning geografik kengligi necha gradusga teng?", correct: "0°", options: ["0°", "90°", "45°", "180°"] },
  { id: 39, q: "Yer sharining qutblarida geografik kenglik necha gradusga teng bo'ladi?", correct: "90°", options: ["90°", "0°", "180°", "60°"] },
  { id: 40, q: "Nuqtaning yer markaziga yo'nalgan shovun chizig'i asosida aniqlangan koordinatasi qaysi?", correct: "Astronomik koordinata", options: ["Astronomik koordinata", "Geodezik koordinata", "To'g'ri burchakli koordinata", "Qutbiy koordinata"] },
  { id: 41, q: "Geodezik koordinatalar qaysi matematik model asosida o'lchanadi?", correct: "Referens-ellipsoid", options: ["Referens-ellipsoid", "Geoid", "Sfera", "Paraboloid"] },
  { id: 42, q: "To'g'ri burchakli koordinatalar sistemasida X o'qi sifatida nima qabul qilinadi?", correct: "Meridian yo'nalishi", options: ["Meridian yo'nalishi", "Parallel yo'nalishi", "Ekvator yo'nalishi", "Magnit shimol"] },
  { id: 43, q: "Qutbiy koordinata sistemasida nuqta o'rni qaysi elementlar bilan aniqlanadi?", correct: "Radius-vektor va mo'ljallash burchagi", options: ["Radius-vektor va mo'ljallash burchagi", "X va Y koordinatalar", "Kenglik va uzunlik", "Azimut va balandlik"] },
  { id: 44, q: "Yer ellipsoidi Grinvich meridianidan boshlab necha gradusli zonalarga bo'linadi?", correct: "6° yoki 3° zonalarga", options: ["6° yoki 3° zonalarga", "10° yoki 5° zonalarga", "15° yoki 7.5° zonalarga", "4° yoki 2° zonalarga"] },
  { id: 45, q: "A va B nuqtalar orasidagi balandliklar farqi (h) nima deb ataladi?", correct: "Nisbiy balandlik", options: ["Nisbiy balandlik", "Mutlaq balandlik", "Geodezik balandlik", "Gipsome trik balandlik"] },
  { id: 46, q: "Geoinformatika fanida LiDAR texnologiyasi nima uchun xizmat qiladi?", correct: "Masofani lazer yordamida o'lchash uchun", options: ["Masofani lazer yordamida o'lchash uchun", "Sun'iy yo'ldoshdan signal olish uchun", "Suv osti topografiyasini o'lchash uchun", "Havo haroratini o'lchash uchun"] },
  { id: 47, q: "O'zbekistonda yer tuzish ishlarini qaysi tashkilot boshqaradi?", correct: "Kadastr agentligi", options: ["Kadastr agentligi", "Yer vazirligi", "O'zdaverloyiha", "Qishloq xo'jaligi vazirligi"] },
  { id: 48, q: "Yer tuzish loyihalarini joyga ko'chirishda asosan kim ishtirok etadi?", correct: "Loyiha muallifi va yer tuzish xizmati", options: ["Loyiha muallifi va yer tuzish xizmati", "Faqat muhandislar", "Kadastr xizmati va politsiya", "Faqat yer egasi"] },
  { id: 49, q: "Yer tuzish loyihasining yozma qismi qanday hujjatdan iborat bo'ladi?", correct: "Tushuntirish xati", options: ["Tushuntirish xati", "Chizma", "Raqamli xarita", "Kadastr pasporti"] },
  { id: 50, q: "AutoCAD dasturida topografik obyektlarni guruhlash uchun nima ishlatiladi?", correct: "Layer", options: ["Layer", "Block", "Polyline", "Region"] },
  { id: 51, q: "Bino va inshootlarning cho'kishini kuzatish nima deb ataladi?", correct: "Geodezik monitoring", options: ["Geodezik monitoring", "Deformatsiya o'lchash", "Tektonik tahlil", "Inshoot nazorati"] },
  { id: 52, q: "Baland inshootlarning egilishini doimiy kuzatish uchun nima o'rnatiladi?", correct: "Geodezik reperlar", options: ["Geodezik reperlar", "Kameralar", "Seysmograflar", "Barometrlar"] },
  { id: 53, q: "UUA (Uchuvchisiz uchish apparatlari) qisqartmasi nimani anglatadi?", correct: "Uchuvchisiz uchish apparatlari", options: ["Uchuvchisiz uchish apparatlari", "Uzoqdan boshqariladigan uskuna", "Ultra uchuvchi apparat", "Universal uchish agregati"] },
  { id: 54, q: "O'zbekistonda yer islohotlari davrida qaysi institut loyihalarni tayyorlaydi?", correct: "O'zdaverloyiha instituti", options: ["O'zdaverloyiha instituti", "Kadastr agentligi", "Geodeziya instituti", "Qishloq xo'jaligi instituti"] },
  { id: 55, q: "Nisbiy balandlikni hisoblash formulasi h = a - b da 'a' nimani bildiradi?", correct: "Orqa reyka sanoq qiymati", options: ["Orqa reyka sanoq qiymati", "Oldingi reyka sanoq qiymati", "Asbob balandligi", "Gorizont instrumenta"] },
  { id: 56, q: "Teodolitda 'limb' qismi nima uchun xizmat qiladi?", correct: "Burchaklarni o'lchash uchun", options: ["Burchaklarni o'lchash uchun", "Masofani o'lchash uchun", "Balandlikni aniqlash uchun", "Nishonni ko'rish uchun"] },
  { id: 57, q: "Geodeziyada 'shovun' (plumb bob) nima maqsadda ishlatiladi?", correct: "Vertikal yo'nalishni aniqlash uchun", options: ["Vertikal yo'nalishni aniqlash uchun", "Gorizontal yo'nalishni aniqlash uchun", "Magnit shimolni aniqlash uchun", "Masofani o'lchash uchun"] },
  { id: 58, q: "Aholi punktlarining 1:500 masshtabdagi rejasi qanday aniqlikda bo'lishi kerak?", correct: "0,5 m aniqlikda", options: ["0,5 m aniqlikda", "1 m aniqlikda", "0,1 m aniqlikda", "2 m aniqlikda"] },
  { id: 59, q: "Yer uchastkasiga bo'lgan ijara huquqi yakka tartibdagi uy-joy uchun necha yil?", correct: "99 yil", options: ["99 yil", "49 yil", "25 yil", "75 yil"] },
  { id: 60, q: "Yer uchastkasiga bo'lgan ijara huquqi tadbirkorlik uchun necha yil etib belgilanadi?", correct: "49 yil", options: ["49 yil", "99 yil", "25 yil", "30 yil"] },
  { id: 61, q: "O'zboshimchalik bilan egallangan yerlarni e'tirof etish muddati qaysi sanagacha?", correct: "2018-yil 1-maygacha", options: ["2018-yil 1-maygacha", "2020-yil 1-yanvargacha", "2015-yil 1-iyulgacha", "2019-yil 1-martgacha"] },
  { id: 62, q: "Yer uchastkasini e'tirof etish uchun bir martalik to'lov Toshkentda qancha?", correct: "BHMning 5 baravari", options: ["BHMning 5 baravari", "BHMning 3 baravari", "BHMning 10 baravari", "BHMning 2 baravari"] },
  { id: 63, q: "Nukus shahri va viloyat markazlarida bir martalik to'lov miqdori qancha?", correct: "BHMning 3 baravari", options: ["BHMning 3 baravari", "BHMning 5 baravari", "BHMning 1 baravari", "BHMning 2 baravari"] },
  { id: 64, q: "I va II guruh nogironligi bo'lgan shaxslar bir martalik to'lovdan qanday foydalanadi?", correct: "To'lovdan ozod etiladi", options: ["To'lovdan ozod etiladi", "50% chegirma oladi", "To'liq to'laydi", "25% chegirma oladi"] },
  { id: 65, q: "Yer uchastkalarini xatlovdan o'tkazish nima asosida amalga oshiriladi?", correct: "Avtomatlashtirilgan axborot tizimi asosida", options: ["Avtomatlashtirilgan axborot tizimi asosida", "Qog'oz hujjatlar asosida", "Shaxsiy muroja'at asosida", "Mahalliy hokimlik qarori asosida"] },
  { id: 66, q: "Kadastr agentligining avtomatlashtirilgan axborot tizimi nima maqsadda ishlaydi?", correct: "Yer huquqlarini e'tirof etish uchun", options: ["Yer huquqlarini e'tirof etish uchun", "Soliq yig'ish uchun", "Qurilish nazorati uchun", "Suv resurslarini boshqarish uchun"] },
  { id: 67, q: "Dronlar yordamida o'simliklar kasalligini aniqlashda qanday kamera ishlatiladi?", correct: "Multispektral kamera", options: ["Multispektral kamera", "Oddiy raqamli kamera", "Infraqizil kamera", "Termal kamera"] },
  { id: 68, q: "Topografik xaritalarda relyef nimalar yordamida tasvirlanadi?", correct: "Gorizontallar yordamida", options: ["Gorizontallar yordamida", "Ranglar yordamida", "Sonlar yordamida", "Belgilar yordamida"] },
  { id: 69, q: "Geodezik punktlar joyda qanday mahkamlanadi?", correct: "Maxsus belgi yoki reper bilan", options: ["Maxsus belgi yoki reper bilan", "Beton ustun bilan", "Metal qoziq bilan", "Daraxt bilan"] },
  { id: 70, q: "Niveller reykasidagi bo'linmalar odatda qanday o'lchamda bo'ladi?", correct: "Santimetr va millimetr bo'linmalarda", options: ["Santimetr va millimetr bo'linmalarda", "Metr bo'linmalarda", "Faqat santimetr bo'linmalarda", "Millimetr bo'linmalarda"] },
  { id: 71, q: "Teodolitda 'optik vizir' nima uchun xizmat qiladi?", correct: "Nishonni aniq ko'rish uchun", options: ["Nishonni aniq ko'rish uchun", "Masofani o'lchash uchun", "Burchakni hisoblash uchun", "Balandlikni aniqlash uchun"] },
  { id: 72, q: "Yer resurslaridan intensiv foydalanish nima degani?", correct: "Kam maydondan ko'proq samara olish", options: ["Kam maydondan ko'proq samara olish", "Ko'p maydon ishlatish", "Yangi yerlar o'zlashtirish", "Yerlarni dam oldirish"] },
  { id: 73, q: "Geodeziyada 'kollimatsion xato' nima bilan bog'liq?", correct: "Vizir o'qi xatosi bilan", options: ["Vizir o'qi xatosi bilan", "Balandlik o'lchash xatosi bilan", "Magnit xato bilan", "Refraktsiya xatosi bilan"] },
  { id: 74, q: "Tuman yer tuzish chizmasi odatda necha yilga mo'ljallanadi?", correct: "10–15 yilga", options: ["10–15 yilga", "5–10 yilga", "20–25 yilga", "25–30 yilga"] },
  { id: 75, q: "Yerlarni rekultivatsiyalash deganda nimani tushunasiz?", correct: "Buzilgan yerlarni tiklash", options: ["Buzilgan yerlarni tiklash", "Yangi yer o'zlashtirish", "Yer solig'ini to'lash", "Yer chegarasini belgilash"] },
  { id: 76, q: "Eroziyaga qarshi tadbirlar qaysi chizmada ko'rsatiladi?", correct: "Yer tuzish chizmasida", options: ["Yer tuzish chizmasida", "Topografik xaritada", "Kadastr xaritasida", "Geologik xaritada"] },
  { id: 77, q: "Mutlaq balandlik va nisbiy balandlik o'rtasidagi farq nima?", correct: "Mutlaq balandlik dengiz sathidan, nisbiy balandlik ikki nuqta orasida aniqlanadi", options: ["Mutlaq balandlik dengiz sathidan, nisbiy balandlik ikki nuqta orasida aniqlanadi", "Mutlaq balandlik tog'dan, nisbiy balandlik dengizdan o'lchanadi", "Ikkalasi ham dengiz sathidan o'lchanadi", "Farq yo'q, bir xil tushuncha"] },
  { id: 78, q: "AutoCAD dasturida 'Polyline' buyrug'i nima uchun kerak?", correct: "Chiziqli obyektlarni chizish uchun", options: ["Chiziqli obyektlarni chizish uchun", "Aylana chizish uchun", "Matn kiritish uchun", "Rangni o'zgartirish uchun"] },
  { id: 79, q: "Geodeziyada 'bussol' asbobi nima uchun ishlatiladi?", correct: "Magnit azimutni aniqlash uchun", options: ["Magnit azimutni aniqlash uchun", "Balandlikni o'lchash uchun", "Masofani o'lchash uchun", "Burchakni o'lchash uchun"] },
  { id: 80, q: "Yer tuzishda 'mualliflik nazorati' kim tomonidan olib boriladi?", correct: "Loyiha muallifi tomonidan", options: ["Loyiha muallifi tomonidan", "Kadastr agentligi tomonidan", "Hokimiyat tomonidan", "Yer egasi tomonidan"] },
  { id: 81, q: "Raqamli topografik reja qaysi formatda saqlanishi mumkin?", correct: "DWG yoki DXF formatida", options: ["DWG yoki DXF formatida", "PDF formatida", "JPEG formatida", "TXT formatida"] },
  { id: 82, q: "'Hikmat uyi' ilmiy markazi qaysi shaharda tashkil etilgan?", correct: "Bag'dodda", options: ["Bag'dodda", "Samarqandda", "Qohirada", "Istanbulda"] },
  { id: 83, q: "Yer siqilishi (α) formulasida 'a' va 'b' nimalar?", correct: "a — katta yarim o'q, b — kichik yarim o'q", options: ["a — katta yarim o'q, b — kichik yarim o'q", "a — radius, b — diametr", "a — kenglik, b — uzunlik", "a — balandlik, b — chuqurlik"] },
  { id: 84, q: "Geodeziyada 'profil' so'zi nimani anglatadi?", correct: "Joyning vertikal kesimi", options: ["Joyning vertikal kesimi", "Joyning gorizontal rejasi", "Yer sirtining surati", "Xaritaning masshtabi"] },
  { id: 85, q: "Teodolitda 'vizir o'qi' nima orqali o'tadi?", correct: "Obyektiv markazi va iplar to'ri markazidan", options: ["Obyektiv markazi va iplar to'ri markazidan", "Faqat obiektiv markazidan", "Okulyar markazidan", "Limb markazidan"] },
  { id: 86, q: "Total stansiya asbobining xotirasidagi ma'lumotlar qanday olinadi?", correct: "USB yoki xotira karta orqali", options: ["USB yoki xotira karta orqali", "Bluetooth orqali", "Wi-Fi orqali", "Qog'ozga chop etish orqali"] },
  { id: 87, q: "Qaysi vaziyatda er uchastkasiga bo'lgan huquq e'tirof etilmaydi?", correct: "Qonun shartlariga mos kelmaganda", options: ["Qonun shartlariga mos kelmaganda", "Yer egasi so'raganda", "Hokimiyat xohlaganda", "Qo'shni rozi bo'lmaganda"] },
  { id: 88, q: "Yer solig'i va mol-mulk solig'i bo'yicha qarzdorlik bo'lsa nima qilinadi?", correct: "Ishlar to'xtatib turiladi", options: ["Ishlar to'xtatib turiladi", "Jarima to'lash talab etiladi", "Yer musodara qilinadi", "Hech narsa qilinmaydi"] },
  { id: 89, q: "Dronlar yordamida qishloq xo'jaligida nima monitoring qilinadi?", correct: "Ekinlar holati va kasalliklari", options: ["Ekinlar holati va kasalliklari", "Ob-havo holati", "Tuproq tarkibi", "Suv manbalari"] },
  { id: 90, q: "Geodezik asboblarni 'kalibrlash' nima degani?", correct: "Asbob aniqligini tekshirib sozlash", options: ["Asbob aniqligini tekshirib sozlash", "Asbobni tozalash", "Asbobni saqlash", "Asbobni ta'mirlash"] },
  { id: 91, q: "Teodolitni tekshirishda 'shovunsiz' usulda nima qo'llaniladi?", correct: "Optik markazlashtirgich", options: ["Optik markazlashtirgich", "Lazer nur", "Magnit kompas", "Darajali pufakcha"] },
  { id: 92, q: "Yer tuzishda 'ichki er tuzish' loyihasi kimlar uchun?", correct: "Xo'jalik ichidagi yer egalari uchun", options: ["Xo'jalik ichidagi yer egalari uchun", "Shahar aholisi uchun", "Sanoat korxonalari uchun", "Davlat muassasalari uchun"] },
  { id: 93, q: "Bino deformatsiyasini kuzatishda 'reper' nima?", correct: "Barqaror balandlik tayanch nuqtasi", options: ["Barqaror balandlik tayanch nuqtasi", "Deformatsiya o'lchagich", "Magnit belgi", "Koordinata nuqtasi"] },
  { id: 94, q: "Google Maps tizimi qaysi koordinata modelidan foydalanadi?", correct: "WGS-84", options: ["WGS-84", "SK-42", "PZ-90", "ITRF"] },
  { id: 95, q: "Yer tuzish loyihasi hayotga tadbiq etilgach nima kuchga kiradi?", correct: "Loyiha hujjatlari kuchga kiradi", options: ["Loyiha hujjatlari kuchga kiradi", "Eski hujjatlar bekor qilinadi", "Yangi o'lchov ishlari boshlanadi", "Kadastr qayta tuziladi"] },
  { id: 96, q: "'Gadus o'lchash usuli' nima maqsadda ishlatilgan?", correct: "Yer o'lchamlarini aniqlash uchun", options: ["Yer o'lchamlarini aniqlash uchun", "Dengiz chuqurligini o'lchash uchun", "Tog' balandligini o'lchash uchun", "Masofa hisoblash uchun"] },
  { id: 97, q: "Yerning matematik shakliga eng yaqin keladigan geometrik shakl?", correct: "Aylanish ellipsoidi", options: ["Aylanish ellipsoidi", "Sfera", "Geoid", "Paraboloid"] },
  { id: 98, q: "Yer sirtining 510 mln km kvadrat maydonidan quruqlik qancha?", correct: "147,9 mln km²", options: ["147,9 mln km²", "200 mln km²", "100 mln km²", "362 mln km²"] },
  { id: 99, q: "Qaysi asbob nur signali (lazer) asosida masofani o'lchaydi?", correct: "Elektron masofa o'lchagich", options: ["Elektron masofa o'lchagich", "Teodolit", "Niveller", "Bussol"] },
  { id: 100, q: "Niveller bilan ishlashda 'gorizont instrumenta' nima?", correct: "Asbob ko'rish nuri balandligi", options: ["Asbob ko'rish nuri balandligi", "Asbob o'rnatilgan nuqta balandligi", "Nishon balandligi", "Reyka nol belgisi balandligi"] },
];

const SECTIONS = [
  { label: "I Qism (1–25)", range: [0, 25] },
  { label: "II Qism (26–50)", range: [25, 50] },
  { label: "III Qism (51–75)", range: [50, 75] },
  { label: "IV Qism (76–100)", range: [75, 100] },
];

function shuffle(arr) {
  const a = [...arr];
  for (let i = a.length - 1; i > 0; i--) {
    const j = Math.floor(Math.random() * (i + 1));
    [a[i], a[j]] = [a[j], a[i]];
  }
  return a;
}

function getResultMessage(score, total) {
  const pct = (score / total) * 100;
  if (pct === 100) return { msg: "🏆 Ajoyib! Siz geodeziya bo'yicha haqiqiy professionalсиз! Barcha savolga to'g'ri javob berdingiz — bu nadir natija!", color: "#22c55e" };
  if (pct >= 85) return { msg: "🌟 Zo'r natija! Bilimingiz juda yaxshi. Siz kelajakda geodeziya sohasida yetuk mutaxassis bo'lasiz!", color: "#16a34a" };
  if (pct >= 70) return { msg: "👍 Yaxshi! Bilimingiz qoniqarli darajada. Bir oz ko'proq o'qisangiz, mukammal natijaga erishasiz!", color: "#ca8a04" };
  if (pct >= 50) return { msg: "📚 O'rtacha natija. Geodeziya fanini qayta o'rganishingiz tavsiya etiladi. Harakatda davom eting!", color: "#f97316" };
  if (pct >= 30) return { msg: "⚠️ Bilimingizni mustahkamlash kerak. Darsliklarni diqqat bilan o'qib chiqing, imtihonga tayyorgarlik ko'ring!", color: "#dc2626" };
  return { msg: "❌ Afsuski, natija past. Lekin xafa bo'lmang! Har bir muvaffaqiyat urinishdan boshlanadi. Qaytadan o'qib chiqing!", color: "#b91c1c" };
}

export default function App() {
  const [screen, setScreen] = useState("home"); // home | test | result
  const [questions, setQuestions] = useState([]);
  const [current, setCurrent] = useState(0);
  const [answers, setAnswers] = useState({});
  const [selected, setSelected] = useState(null);
  const [confirmed, setConfirmed] = useState(false);
  const [sectionMode, setSectionMode] = useState(null);
  const [shuffledOptions, setShuffledOptions] = useState([]);

  const startTest = useCallback((mode) => {
    let qs;
    if (mode === "random30") {
      qs = shuffle(ALL_QUESTIONS).slice(0, 30);
    } else {
      const [s, e] = SECTIONS[mode].range;
      qs = shuffle(ALL_QUESTIONS.slice(s, e));
    }
    setSectionMode(mode);
    setQuestions(qs);
    setAnswers({});
    setCurrent(0);
    setSelected(null);
    setConfirmed(false);
    setScreen("test");
  }, []);

  useEffect(() => {
    if (questions.length > 0 && questions[current]) {
      setShuffledOptions(shuffle(questions[current].options));
      setSelected(null);
      setConfirmed(false);
    }
  }, [current, questions]);

  const handleSelect = (opt) => {
    if (!confirmed) setSelected(opt);
  };

  const handleConfirm = () => {
    if (!selected) return;
    setConfirmed(true);
    setAnswers(prev => ({ ...prev, [current]: selected }));
  };

  const handleNext = () => {
    if (current + 1 < questions.length) {
      setCurrent(c => c + 1);
    } else {
      setScreen("result");
    }
  };

  const score = Object.entries(answers).filter(([i, a]) => questions[i] && a === questions[i].correct).length;

  if (screen === "home") {
    return (
      <div style={{
        minHeight: "100vh",
        background: "linear-gradient(135deg, #0f0f0f 0%, #1a0a0a 40%, #0a1a0a 100%)",
        fontFamily: "'Georgia', serif",
        padding: "0 0 40px 0",
      }}>
        {/* Header */}
        <div style={{
          background: "linear-gradient(90deg, #8b0000, #2d6a2d)",
          padding: "24px 20px 16px",
          textAlign: "center",
          borderBottom: "3px solid #d4a800",
          boxShadow: "0 4px 20px rgba(0,0,0,0.5)",
        }}>
          <div style={{ display: "flex", alignItems: "center", justifyContent: "center", gap: 12, marginBottom: 6 }}>
            <span style={{ fontSize: 28 }}>🎓</span>
            <div>
              <div style={{ color: "#ffd700", fontSize: 13, fontWeight: "bold", letterSpacing: 1, textTransform: "uppercase" }}>Buxoro davlat texnika universiteti</div>
              <div style={{ color: "#fff", fontSize: 20, fontWeight: "bold", lineHeight: 1.2 }}>Yer tuzishda geodezik ishlar</div>
              <div style={{ color: "#a8d8a8", fontSize: 12, marginTop: 2 }}>Test tizimi — 100 ta savol</div>
            </div>
          </div>
          <div style={{ color: "#ffcccb", fontSize: 11, marginTop: 4 }}>Tuzuvchi: Normamatov A</div>
        </div>

        <div style={{ maxWidth: 500, margin: "0 auto", padding: "24px 16px" }}>
          <div style={{
            background: "rgba(255,255,255,0.05)",
            border: "1px solid rgba(255,215,0,0.3)",
            borderRadius: 12,
            padding: "16px",
            marginBottom: 20,
            textAlign: "center",
          }}>
            <div style={{ color: "#ffd700", fontSize: 14, marginBottom: 6 }}>📋 Test bo'limlari</div>
            <div style={{ color: "#ccc", fontSize: 12, lineHeight: 1.6 }}>
              Har bir bo'lim 25 ta savoldan iborat.<br />
              Savollar va javoblar har safar tasodifiy tartibda chiqadi.
            </div>
          </div>

          {/* Section buttons */}
          {SECTIONS.map((sec, i) => (
            <button
              key={i}
              onClick={() => startTest(i)}
              style={{
                width: "100%",
                padding: "14px 20px",
                marginBottom: 10,
                background: i % 2 === 0
                  ? "linear-gradient(90deg, #8b0000 0%, #c0392b 100%)"
                  : "linear-gradient(90deg, #1a5c1a 0%, #27ae60 100%)",
                border: "none",
                borderRadius: 10,
                color: "#fff",
                fontSize: 15,
                fontWeight: "bold",
                cursor: "pointer",
                display: "flex",
                alignItems: "center",
                justifyContent: "space-between",
                boxShadow: "0 3px 10px rgba(0,0,0,0.4)",
                transition: "transform 0.1s, opacity 0.1s",
              }}
              onMouseEnter={e => e.currentTarget.style.opacity = "0.85"}
              onMouseLeave={e => e.currentTarget.style.opacity = "1"}
            >
              <span>📚 {sec.label}</span>
              <span style={{ background: "rgba(255,255,255,0.2)", padding: "2px 10px", borderRadius: 20, fontSize: 12 }}>25 ta savol →</span>
            </button>
          ))}

          {/* Random 30 */}
          <button
            onClick={() => startTest("random30")}
            style={{
              width: "100%",
              padding: "16px 20px",
              marginTop: 6,
              background: "linear-gradient(90deg, #d4a800, #ff6b00)",
              border: "none",
              borderRadius: 10,
              color: "#000",
              fontSize: 15,
              fontWeight: "bold",
              cursor: "pointer",
              display: "flex",
              alignItems: "center",
              justifyContent: "space-between",
              boxShadow: "0 4px 15px rgba(212,168,0,0.4)",
              transition: "transform 0.1s",
            }}
            onMouseEnter={e => e.currentTarget.style.opacity = "0.85"}
            onMouseLeave={e => e.currentTarget.style.opacity = "1"}
          >
            <span>⚡ Tezkor tasodifiy 30 ta savol</span>
            <span style={{ background: "rgba(0,0,0,0.2)", padding: "2px 10px", borderRadius: 20, fontSize: 12 }}>Barcha qismdan →</span>
          </button>

          <div style={{ marginTop: 20, padding: 12, background: "rgba(255,255,255,0.04)", borderRadius: 8, textAlign: "center" }}>
            <div style={{ color: "#888", fontSize: 11, lineHeight: 1.7 }}>
              Har bir test yakunida natijangiz va izoh ko'rsatiladi.<br />
              Muvaffaqiyatlar! 🌿
            </div>
          </div>
        </div>
      </div>
    );
  }

  if (screen === "test") {
    const q = questions[current];
    const total = questions.length;
    const progress = ((current) / total) * 100;

    return (
      <div style={{
        minHeight: "100vh",
        background: "linear-gradient(135deg, #0f0f0f, #1a0a0a, #0a1a0a)",
        fontFamily: "'Georgia', serif",
      }}>
        {/* Header */}
        <div style={{
          background: "linear-gradient(90deg, #8b0000, #2d6a2d)",
          padding: "12px 16px",
          borderBottom: "3px solid #d4a800",
        }}>
          <div style={{ color: "#ffd700", fontSize: 12, fontWeight: "bold", textAlign: "center", letterSpacing: 1 }}>
            BUXORO DAVLAT TEXNIKA UNIVERSITETI
          </div>
          <div style={{ color: "#fff", fontSize: 11, textAlign: "center", marginTop: 2 }}>
            {sectionMode === "random30" ? "⚡ Tezkor 30 ta Savol" : SECTIONS[sectionMode]?.label}
          </div>
        </div>

        {/* Progress */}
        <div style={{ padding: "10px 16px 0" }}>
          <div style={{ display: "flex", justifyContent: "space-between", marginBottom: 4 }}>
            <span style={{ color: "#aaa", fontSize: 12 }}>Savol {current + 1} / {total}</span>
            <span style={{ color: "#d4a800", fontSize: 12 }}>
              ✅ {Object.values(answers).filter((a, i) => questions[i] && a === questions[i].correct).length} to'g'ri
            </span>
          </div>
          <div style={{ background: "#333", borderRadius: 6, height: 8, overflow: "hidden" }}>
            <div style={{
              height: "100%",
              width: `${progress}%`,
              background: "linear-gradient(90deg, #8b0000, #d4a800, #2d6a2d)",
              transition: "width 0.4s",
              borderRadius: 6,
            }} />
          </div>
        </div>

        {/* Question */}
        <div style={{ padding: "16px" }}>
          <div style={{
            background: "rgba(255,255,255,0.07)",
            border: "1px solid rgba(212,168,0,0.4)",
            borderRadius: 12,
            padding: "16px",
            marginBottom: 14,
          }}>
            <div style={{ color: "#d4a800", fontSize: 11, marginBottom: 6, letterSpacing: 1 }}>
              SAVOL {q.id}
            </div>
            <div style={{ color: "#fff", fontSize: 15, lineHeight: 1.5 }}>
              {q.q}
            </div>
          </div>

          {/* Options */}
          {shuffledOptions.map((opt, idx) => {
            let bg = "rgba(255,255,255,0.06)";
            let border = "1px solid rgba(255,255,255,0.1)";
            let col = "#ddd";
            let icon = ["A", "B", "C", "D"][idx];

            if (confirmed) {
              if (opt === q.correct) {
                bg = "rgba(34,197,94,0.2)";
                border = "2px solid #22c55e";
                col = "#4ade80";
                icon = "✓";
              } else if (opt === selected && opt !== q.correct) {
                bg = "rgba(239,68,68,0.2)";
                border = "2px solid #ef4444";
                col = "#f87171";
                icon = "✗";
              }
            } else if (opt === selected) {
              bg = "rgba(212,168,0,0.2)";
              border = "2px solid #d4a800";
              col = "#ffd700";
            }

            return (
              <button
                key={opt}
                onClick={() => handleSelect(opt)}
                style={{
                  width: "100%",
                  padding: "12px 14px",
                  marginBottom: 8,
                  background: bg,
                  border,
                  borderRadius: 10,
                  color: col,
                  fontSize: 14,
                  cursor: confirmed ? "default" : "pointer",
                  display: "flex",
                  alignItems: "center",
                  gap: 10,
                  textAlign: "left",
                  transition: "all 0.2s",
                }}
              >
                <span style={{
                  minWidth: 24, height: 24,
                  borderRadius: "50%",
                  background: confirmed && opt === q.correct ? "#22c55e" :
                    confirmed && opt === selected && opt !== q.correct ? "#ef4444" :
                      opt === selected ? "#d4a800" : "rgba(255,255,255,0.15)",
                  display: "flex", alignItems: "center", justifyContent: "center",
                  fontSize: 12, fontWeight: "bold", color: "#fff",
                  flexShrink: 0,
                }}>
                  {icon}
                </span>
                <span>{opt}</span>
              </button>
            );
          })}

          {/* Action buttons */}
          <div style={{ marginTop: 8 }}>
            {!confirmed ? (
              <button
                onClick={handleConfirm}
                disabled={!selected}
                style={{
                  width: "100%",
                  padding: "14px",
                  background: selected ? "linear-gradient(90deg, #8b0000, #c0392b)" : "#333",
                  border: "none",
                  borderRadius: 10,
                  color: selected ? "#fff" : "#666",
                  fontSize: 15,
                  fontWeight: "bold",
                  cursor: selected ? "pointer" : "not-allowed",
                  transition: "all 0.2s",
                }}
              >
                ✔ Javobni tasdiqlash
              </button>
            ) : (
              <button
                onClick={handleNext}
                style={{
                  width: "100%",
                  padding: "14px",
                  background: current + 1 < total
                    ? "linear-gradient(90deg, #1a5c1a, #27ae60)"
                    : "linear-gradient(90deg, #d4a800, #ff8c00)",
                  border: "none",
                  borderRadius: 10,
                  color: current + 1 < total ? "#fff" : "#000",
                  fontSize: 15,
                  fontWeight: "bold",
                  cursor: "pointer",
                }}
              >
                {current + 1 < total ? "Keyingi savol →" : "🏁 Natijani ko'rish"}
              </button>
            )}
          </div>

          <button
            onClick={() => setScreen("home")}
            style={{
              width: "100%",
              padding: "10px",
              marginTop: 8,
              background: "transparent",
              border: "1px solid #444",
              borderRadius: 8,
              color: "#888",
              fontSize: 12,
              cursor: "pointer",
            }}
          >
            ← Bosh sahifaga qaytish
          </button>
        </div>
      </div>
    );
  }

  // Result screen
  const total = questions.length;
  const pct = Math.round((score / total) * 100);
  const result = getResultMessage(score, total);

  const wrong = questions.filter((q, i) => answers[i] && answers[i] !== q.correct);
  const unanswered = total - Object.keys(answers).length;

  return (
    <div style={{
      minHeight: "100vh",
      background: "linear-gradient(135deg, #0f0f0f, #1a0a0a, #0a1a0a)",
      fontFamily: "'Georgia', serif",
      paddingBottom: 40,
    }}>
      <div style={{
        background: "linear-gradient(90deg, #8b0000, #2d6a2d)",
        padding: "16px",
        borderBottom: "3px solid #d4a800",
        textAlign: "center",
      }}>
        <div style={{ color: "#ffd700", fontSize: 13, fontWeight: "bold" }}>BUXORO DAVLAT TEXNIKA UNIVERSITETI</div>
        <div style={{ color: "#fff", fontSize: 18, fontWeight: "bold" }}>📊 Test Natijasi</div>
        <div style={{ color: "#a8d8a8", fontSize: 11 }}>Tuzuvchi: Normamatov A</div>
      </div>

      <div style={{ maxWidth: 500, margin: "0 auto", padding: "20px 16px" }}>
        {/* Score circle */}
        <div style={{ textAlign: "center", marginBottom: 20 }}>
          <div style={{
            width: 120, height: 120,
            borderRadius: "50%",
            background: `conic-gradient(${pct >= 70 ? "#22c55e" : pct >= 50 ? "#f97316" : "#ef4444"} ${pct * 3.6}deg, #222 0deg)`,
            display: "inline-flex", alignItems: "center", justifyContent: "center",
            boxShadow: `0 0 30px ${pct >= 70 ? "rgba(34,197,94,0.4)" : "rgba(239,68,68,0.4)"}`,
            margin: "0 auto",
          }}>
            <div style={{
              width: 90, height: 90, borderRadius: "50%",
              background: "#111",
              display: "flex", alignItems: "center", justifyContent: "center", flexDirection: "column",
            }}>
              <div style={{ color: result.color, fontSize: 22, fontWeight: "bold" }}>{pct}%</div>
              <div style={{ color: "#aaa", fontSize: 10 }}>{score}/{total}</div>
            </div>
          </div>
        </div>

        {/* Stats */}
        <div style={{
          display: "grid", gridTemplateColumns: "1fr 1fr 1fr",
          gap: 8, marginBottom: 16,
        }}>
          {[
            { label: "To'g'ri", val: score, color: "#22c55e", icon: "✅" },
            { label: "Noto'g'ri", val: wrong.length, color: "#ef4444", icon: "❌" },
            { label: "Javobsiz", val: unanswered, color: "#f97316", icon: "⚠️" },
          ].map(s => (
            <div key={s.label} style={{
              background: "rgba(255,255,255,0.06)",
              border: `1px solid ${s.color}44`,
              borderRadius: 10, padding: "12px 8px", textAlign: "center",
            }}>
              <div style={{ fontSize: 18 }}>{s.icon}</div>
              <div style={{ color: s.color, fontSize: 20, fontWeight: "bold" }}>{s.val}</div>
              <div style={{ color: "#888", fontSize: 11 }}>{s.label}</div>
            </div>
          ))}
        </div>

        {/* Result message */}
        <div style={{
          background: `${result.color}15`,
          border: `2px solid ${result.color}55`,
          borderRadius: 12, padding: 16, marginBottom: 16, textAlign: "center",
        }}>
          <div style={{ color: result.color, fontSize: 14, lineHeight: 1.6 }}>{result.msg}</div>
        </div>

        {/* Wrong answers review */}
        {wrong.length > 0 && (
          <div style={{ marginBottom: 16 }}>
            <div style={{ color: "#ef4444", fontSize: 13, fontWeight: "bold", marginBottom: 8 }}>
              ❌ Noto'g'ri javoblar ({wrong.length} ta):
            </div>
            {wrong.map((q) => (
              <div key={q.id} style={{
                background: "rgba(239,68,68,0.08)",
                border: "1px solid rgba(239,68,68,0.3)",
                borderRadius: 8, padding: 10, marginBottom: 6,
              }}>
                <div style={{ color: "#fca5a5", fontSize: 12, marginBottom: 4 }}>S{q.id}: {q.q}</div>
                <div style={{ color: "#22c55e", fontSize: 12 }}>✓ To'g'ri: {q.correct}</div>
              </div>
            ))}
          </div>
        )}

        {/* Buttons */}
        <button
          onClick={() => startTest(sectionMode)}
          style={{
            width: "100%", padding: 14, marginBottom: 8,
            background: "linear-gradient(90deg, #8b0000, #c0392b)",
            border: "none", borderRadius: 10,
            color: "#fff", fontSize: 14, fontWeight: "bold", cursor: "pointer",
          }}
        >
          🔄 Qaytadan urinish
        </button>
        <button
          onClick={() => setScreen("home")}
          style={{
            width: "100%", padding: 14,
            background: "linear-gradient(90deg, #1a5c1a, #27ae60)",
            border: "none", borderRadius: 10,
            color: "#fff", fontSize: 14, fontWeight: "bold", cursor: "pointer",
          }}
        >
          🏠 Bosh sahifaga
        </button>
      </div>
    </div>
  );
}
