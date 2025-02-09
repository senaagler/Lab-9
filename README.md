# Lab-9
Hotel
#include <stdio.h>
#include <stdlib.h>
#include <string.h>
#include <math.h>

struct oda{

int odanumarasi;
int yataksayisi;
float ucret;
char *manzara[50];

};

struct musteri{

    char *musteriadi[100];
    struct oda x;
    char *giristarihi[20];
    char *cikistarihi[20];
    float toplamucret;
};



struct tarih{
int gun;
int ay;
int yil;
};



void rezervasyonekle()
{
    struct oda y;
    struct musteri b;
    printf("Oda numarasini,yatak sayisini,ucret,manzara  giriniz:\n");
    scanf("%d %d %f %s",&y.odanumarasi,&y.yataksayisi,&y.ucret,&y.manzara);


    printf("\n Musteri adi,giris tarihi,cikis tarihi:\n");
    scanf("%s %s %s",b.musteriadi,b.giristarihi,b.cikistarihi);


}

void rezervasyonlistele(){

   struct oda;
   struct musteri;
}


void odanumarasiara(int odanumarasi)
{
    struct oda;
    printf("Aranacak oda numarasini giriniz:\n");
    scanf("%d",&odanumarasi);
    printf("bulunan odalar:strstr(%d)");
}



void giristarihisirala()
{
    struct musteri;
    int g;
    int a;
    int y;
    struct tarih t;
    t.gun=g;
    t.ay=a;
    t.yil=y;
    printf("tarihi girin:\n");
    scanf("%d%d%d",t.gun,t.ay,t.yil);

}

int main()
{
int secim;

printf("-------OTEL REZARVASYON SİİSTEMİ-------");
printf("1.Rezarvasyon ekle\n");
printf("2.Rezarvasyonlari listele\n");
printf("3.Oda numarasina gore Ara\n");
printf("4.Cikis\n");

printf("Lutfen secim yapiniz:\n");
scanf("%d",&secim);


switch(secim)
{
    case 1:printf("Yeni musteri ekleyin");
    struct musteri;
    rezervasyonlistele;
    break;

    case 2:printf("Tum rezervasyonlar:\n");
    struct oda;
    rezervasyonekle;
    break;

    case 3:printf("Aranacak oda numarasini giriniz:\n");
    printf("Oda numarasi %d olan odalar strstr(%d)");
    break;

    case 4:printf("Giris tarihine gore siralaniyor...\n");
    giristarihisirala;
    break;


    case 5:printf("cikis\n");break;

    default:printf("gecersiz secim\n");


}
struct oda k;
struct musteri m;

            printf("Musteri Adi: %s\n",k.musteriadi);
            printf("Oda Numarasi: %d\n",k.odanumarasi);
            printf("Yatak Sayisi: %d\n",k.yataksayisi);
            printf("Ucret: %.2f\n",k.ucret);
            printf("Manzara: %s\n",k.manzara);
            printf("Giris Tarihi: %s\n",m.giristarihi);
            printf("Cikis Tarihi: %s\n",m.cikistarihi);
            printf("Toplam Ucret: %.2f\n\n",m.toplamucret);


    return 0;
}


