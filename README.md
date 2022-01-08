#(20 puan) Kullanıcıdan alınan sayısal olarak girilen gün-ay-yıl
# (ör. 04-05-2020) verisini ay verisini metin olacak şekilde (ör.4 Mayıs 2020)
# ekrana yazdıracak kodu yazın. (20 puan)

l={1: "ocak", 2: "şubat", 3: "mart", 4: "nisan", 5: "mayıs",
          6: "haziran", 7: "temmuz", 8: "agustos", 9: "eylül", 10: "ekim" , 11: "kasım" , 12: "aralık"}
print("Tarih verisini giriniz")
u=int(input("30 GÜN İÇERİSİNDEN BİR GÜNÜ SAYI ILE YAZDIRINIZ:"))
if u>30:
    breakpoint("31 Den küçük deger giriniz")
t=int(input("12 AYDAN 1 TANESİNİ SAYI SEKLINDE YAZDIRINIZ:"))
if t>12:
    breakpoint("13 Den küçük bir deger giriniz")
f=int(input("İstediğiniz Yılı yazdiriniz"))
print("Yazdırdığınız tarih:",u,l[t],f,sep="-")



#(30 puan) Aşağıda verilen  f fonksiyonunu kullanıcıdan girilen değere göre hesaplayan programı yazınız

l=int(input("(-1)ile 16 Arasında bir sayı giriniz:"))
if 0<l<9 :
    def u(n):
        if n==1:
            return 1
        return n*u(n-1)
    print(3*u(l))
elif 9<=l<16 :
    t=0
    for i in range(1,l*2):
        if(i%2==0):
            t+=i
            print("Toplam {0}".format(t))
else:
    print("Lütfen geçerli bir aralık giriniz")

#3. (30 puan) Aşağıdaki A şifreleme matrisini kullanarak adınızı ve
# soyadınızı şifreleyen bir program yazın. Şifre sonucunu ekrana yazdırın.
L = {"a": 1, "b": 2, "c": 3, "d": 4, "e": 5, "f": 6, "g": 7, "h": 8, "i": 9, "j": 10, "k": 11, "l": 12, "m": 13,
          "n": 14, "o": 15, "p": 16, "q": 17, "r": 18, "s": 19, "t": 20, "u": 21, "v": 22, "w": 23, "x": 24, "y": 25,
          "z": 26}

u = [[1, 2, -1],
     [2, 5, 2],
     [-1, -2, 2]]

t = [[12, 21, 20],  # lutfugursese
     [6, 21, 7],
     [21, 18, 19]
     [5,19,5]]
result = [[0, 0, 0],
          [0, 0, 0],
          [0, 0, 0]]

    for i in range(len(t[0])):
        for g in range(len(t)):
            result[f][i] += u[f][g] * t[g][i]
for u in result:
    print(u)



#4. 1’den öğrenci numaranızın son iki hanesine kadar arada kalan bütün
# asal sayıları hesaplayabilen bir program yazın. Programda bulunan asal
#sayıları bir list tipinde diziye ekleyin ve bu diziyi ekrana yazdırın.
#okulno1904107503

for l in range(0,3 + 1):
   if l > 1:
       for i in range(2,l):
           if (l % i) == 0:
               break
       else:

        u=[]
        u.append(l)
        print(l)
