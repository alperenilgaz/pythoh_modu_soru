# pythoh_modul_soru
## Programlama Ödevi - Modüller
Proje 1:
--------------
Math modülündeki hazır fonksiyonları kullanarak gelişmiş bir hesap makinesi geliştirmeye çalışın.

cevap :
-------
import math

print("""********************************
işemler
-------
1)karakök alma için 1'e basın.
2)bölümden kalan bulma için 2'ye basın.
3)mutlak değer alma için 3'e basın.
4)üs alma için 4'e basın.

********************************""")
hatalı_seçim=3
while True:
    seçim=input("hangi işlemi kullanmak istiyorsunuz :")
    if(seçim=="q"):
        print("program sonlandırılıyor...")
        break

    elif(seçim=="1"):
        a=int(input("bir sayı giriniz :"))
        print(math.sqrt(a))
    elif(seçim=="2"):
        a = int(input("birinci sayıyı giriniz :"))
        b = int(input("ikinci sayıyı giriniz :"))
        print(math.fmod(a,b))
    elif(seçim=="3"):
        a = int(input("bir sayı giriniz :"))
        print(math.fabs(a))
    elif(seçim=="4"):
        a = int(input("birinci sayıyı giriniz :"))
        b = int(input("ikinci sayıyı giriniz :"))
        print(math.pow(a,b))
    else:
        print("hatalı işlem seçtiniz. Lütfen tekrar seçim yapınız ")
        hatalı_seçim-=1
        if(hatalı_seçim==0):
            print("bilader dalga mı geçiyorsun ikile")
            break

