# Powerbi-Proje
Hotel_Bookings 
Kullanılan Daxlar
1-Ciro_Toplami = CALCULATE(SUMX(hotel_bookings , hotel_bookings[ortalama_gunluk_fiyat] * (hotel_bookings[hafta_ici_gece_kalma] + hotel_bookings[hafta_sonu_gece_kalma]) ), hotel_bookings[iptal_hali]=0) 
2-City Toplam Rezervasyon Sayısı = 
CALCULATE(
    COUNTROWS('hotel_bookings'),
    'hotel_bookings'[otel] = "city")
    
