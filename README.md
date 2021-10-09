________________________________________C++___________________________________________________

#include <iostream>

using namespace std;

int main() {
	
	int a = 42;
	float b = 3.52;
	double c = 4.12234234;
	char d = 65;//acsi kodu
	bool e =false;
	
	cout <<"a"<<a<<endl;
	cout <<"b"<<b<<endl;
	cout <<"c"<<c<<endl;
	cout <<"d"<<d<<endl;
	cout <<"e"<<e<<endl;
	
	
	
	
	return 0;
}


___________________________________________________________________________________________________________________


#include <iostream>

using namespace std;

int main() {
	

	
	int a,b,c,toplam = 0;
	a=1;
	b=2;
	c=3;
	
	toplam = a + b+ c;
	
cout<<" tooplam ; "<<toplam<<endl;
	
	
	
	
	return 0;
}



___________________________________________________________________________________________________________________


#include <iostream>

using namespace std;

int main() {
    
    int a =9;
    cout<<"a degeri"<<a<<endl;
    a+=9; //a nın değerinni 9 arttırır
    cout<<"a degeri"<<a<<endl;
    a++; //a nın değerini 1 arttırır
        cout<<"a degeri"<<a<<endl;
        a--;//a nını değerini 1 azaltır
            cout<<"a degeri"<<a<<endl;
	
	return 0;
}


___________________________________________________________________________________________________________________



#include <iostream>

using namespace std;

int main() {
	int x;
     cout<<"sayi giriniz --";
     cin>>x;
     
     cout<<"girdiğiniz sayi bu mu  -->"<<x<<endl;
     
	return 0;
}

___________________________________________________________________________________________________________________

#include <iostream>

using namespace std;

int main() {


	int a,b,c;
	
	cout<<"1.sayiyi giriniz"<<endl;
	cin>>a;
    cout<<"2.sayiyi giriniz"<<endl;
    cin>>b;
    cout<<"3.sayiyi giriniz"<<endl;
    cin>>c;
	cout<<"toplaminiz-->"<<a+b+c<<endl;

	return 0;
}

___________________________________________________________________________________________________________________

#include <iostream>

using namespace std;

int main() {


	int a,b,c;
	
	cout<<"Sayılari giriniz"<<endl;
	cin>>a>>b>>c;
  	cout<<"toplaminiz-->"<<a+b+c<<endl;

	return 0;
}
___________________________________________________________________________________________________________________

#include <iostream>

using namespace std;

int main() {

  string dk1 = "bu bir foktur";
  string dk2 = " bu bir akdeniz fokudur";
  string dk3 = dk1 + dk2;
  cout<<"string 1 -->"<<dk1<<endl;
  cout<<"string 2 -->"<<dk2<<endl;
  cout<<"string 3 -->"<<dk3<<endl;
	return 0;
}
___________________________________________________________________________________________________________________
//WHİLE İÇİN KOŞUL GEREKİR
#include <iostream>

using namespace std;

int main() {
int i =0;

while(i<100){
	cout<<"i-->"<<i<<endl;
	i++;
}

	return 0;
}
___________________________________________________________________________________________________________________

#include <iostream>

using namespace std;

int main() {
int i =0;
int h;
cout<<"Akacak sayi girin";//bu program alınacak sayıya kadar 0 dan itibaren tüm sayıları ekrana sırasıyla yazdırır.
cin>>h;
while(i<h){
	cout<<"i-->"<<i<<endl;
	i++;
}

	return 0;
}
___________________________________________________________________________________________________________________
//2 değilkenli while örnek
#include <iostream>

using namespace std;

int main() {
int i =0;
int a =0;
while(i<10067 && a<1034){
	cout<<"i-->"<<i<< "a -->" << a<<endl;
	i++;
	a++;
}

	return 0;
}
___________________________________________________________________________________________________________________
//parolayı doğru yazana kadar parola sorar
#include <iostream>

using namespace std;

int main() {

string parla = "144";
string input;

 do{
 	cout<<"parola girin";
 	cin>>input;
 	
 }while(input != parla);

cout<<"parola dogru";

	return 0;
}
___________________________________________________________________________________________________________________

#include <iostream>

using namespace std;

int main() {

string parla = "144";
string input;

 do{
 	cout<<"parola girin";
 	cin>>input;
 
	if(input!=parla){
 		cout<<"parola yanlıs"<<endl;
 		 }
 }while(input != parla);

cout<<"parola dogru";

return 0;

}
___________________________________________________________________________________________________________________

#include <iostream>

using namespace std;

int main() {

int a;
int b;
cout<<"Sayi giriniz=:";
cin>>b;
for(a=0;a<b;a=a+1){
	cout<<"a -->"<<a<<endl;

}

return 0;

}
___________________________________________________________________________________________________________________
//burada int forun içinde kullandık böylece a değeri for döngüsünün içinde ydoğdu yaşadı ve öldü
#include <iostream>

using namespace std;

int main() {


int b;
cout<<"Sayi giriniz=:";
cin>>b;
for(int a=0;a<b;a=a+1){
	cout<<"a -->"<<a<<endl;

}

return 0;

}
___________________________________________________________________________________________________________________

#include <iostream>

using namespace std;

int main() {


int mahmut;
int kale=1;
cout<<"Faktoriyel hesabi icin sayi gir::";
cin>>mahmut;

for(int a=1;a<=mahmut;a++){
	kale *=a ;
	

}
	cout<<mahmut<<" sayisinin faktoriyeli "<<kale<<endl;

return 0;

}
___________________________________________________________________________________________________________________

//Break döngüyü sonlandırır
//Continue döndüyü başa alır 

#include <iostream>

using namespace std;

int main() {

string hakan="danyel";
string tu="1881";
string ad;
string pas;


while(true){
cout<<"Kullanici adi giriniz";
cin>>ad;

cout<<"Parola giriniz";
cin>>pas;
	if (ad==hakan && pas==tu) {
		cout<<"hosgeldiniz"<<endl;
	    break;
		}
	else if(ad!=hakan && pas==tu){
	cout<<"kullanici adı hatalı"<<endl;	
	}
    else if(ad==hakan && pas!=tu){
	cout<<"sifre hatali"<<endl;
	
	}
	else
	cout<<"sg ikiside yanlıs"<<endl;
}

return 0;

}

//alttaki daha iyi
___________________________________________________________________________________________________________________
 #include <iostream>



/* run this p rogram using the console pauser or add your own getch, system("pause") or input loop */

using namespace std;



int main(int argc, char** argv) {

string sys_username ="danyel_karyeli";

string sys_password = "1881"; 



string username;

string password;



cout<<"kullanici adi girniz  ";

cin>> username;

cout<<"parola girin  ";

cin >> password;

if(sys_username == username && sys_password == password){

	cout<<"uzaylilar hos geldiniz"<<endl;
}

else if(sys_username == username && sys_password != password){

	cout<<"sifre yanlis"<<endl;

} else if(sys_username != username && sys_password == password){

	cout<<"kullanici adini yanlis girdin"<<endl;

} else if(sys_username != username && sys_password != password){

	cout<<"kimsin lan sen hem sifre hem kullanici adi yanlis"<<endl;


}

	return 0;

	

	

	

	

}
___________________________________________________________________________________________________________________

#include <iostream>

using namespace std;

int main() {

 int array[3];
 array[0]=10;
 array[1]=20;
 array[2]=30;
 
  cout<<"0.index : "<<array[0]<<endl;
    cout<<"1.index : "<<array[1]<<endl;
      cout<<"2.index : "<<array[2]<<endl;
      
return 0;

}
___________________________________________________________________________________________________________________
 #include <iostream>

using namespace std;

int main() {

double array2[]={1.2,2.4,4.8,9.6};

for(int i = 0;i<4;i++){
	cout<<i<<".ci indeks degeri-->"<<array2[i]<<endl;
}

return 0;

}
___________________________________________________________________________________________________________________

#include <iostream>

using namespace std;

int main() {

string array2[4];

for(int i = 0;i<4;i++){
	cin>>array2[i];
	
}

 for (int i = 0;i<4;i++){
 		cout<<i<<".ci indeks degeri-->"<<array2[i]<<endl;

 }
return 0;

}
___________________________________________________________________________________________________________________

#include <iostream>

using namespace std;

int main() {
 
int java;
 
cout<<"Secenek giriniz (1-2-3-4)";
cin>>java;
 
switch(java){
 
 
case 1:
cout<<"1.islem basliyor..."<<endl;
break;
  
case 2:
cout<<"2.islem basliyor..."<<endl;
break;

case 3:
cout<<"3.islem basliyor..."<<endl;
break;

case 4:
cout<<"4.islem basliyor..."<<endl;
break;

default:
cout<<"1-2-3-4 dedik okuman yazman yok mu!"<<endl;
break;
 }


return 0;
}

___________________________________________________________________________________________________________________

#include <iostream>

using namespace std;

void bay(){
	cout<<"naber ?"<<endl;
	cout<<"iyi misin?"<<endl;
	}


int main() {
 
bay(); //fonsksyon çağırısı
bay();

return 0;
}


___________________________________________________________________________________________________________________

#include <iostream>

using namespace std;

void hatay();


int main() {
 
hatay(); //fonsksyon çağırısı
hatay();

return 0;
}
void hatay(){
	cout<<"naber ?"<<endl;
	cout<<"iyi misin?"<<endl;
	}

___________________________________________________________________________________________________________________

#include <iostream>

using namespace std;

void faktor(int sayi){
	int faktor=1;
	for (int i = 2 ; i<=sayi ; i++){
		faktor*=i;
		
		
	}
	cout<<"faktoriyel--> "<<faktor<<endl;
}


int main() {
	int patates;
cout<<"sayi giriniz"<<endl;
cin>>patates;

faktor(patates);
 

return 0;
}

___________________________________________________________________________________________________________________
//burada return kullandık
#include <iostream>

using namespace std;

int toplam(int a,int b,int c){
	
	return a+b+c;
}


int main() {
int a=toplam(23,23,3);
cout<<"cevap veriyorum --> "<<a<<endl;
return 0;
}

___________________________________________________________________________________________________________________

//KONU DIŞI İNTERNETTE GÖRDÜĞÜM BİR KOD C KODUU FİBONACCİ 

#include <iostream>

using namespace std;


int main(void) {
int x,y,z;

while (1){
	x=0;
	y=1;
	do{
		printf("%d\n",x);
		
	z=x+y;
	x=y;
	y=z;
	
	} while(x<255);
}
return 0;
}


___________________________________________________________________________________________________________________
 //GÖRÜNÜŞE GÖRE AYRI SATIRLARDA YAZMAK ZORUNDA DEĞİLMİŞİZ 

#include <iostream> 
using namespace std;int main() {int x; x=3; cout<<"deger--> "<<x<<endl;}
___________________________________________________________________________________________________________________

#include <iostream> 
using namespace std;
int main() {
string x;
string y;
string z;
 x=3;
  cout<<"Merhaba ben Koni"<<endl;
  cout<<"Senin adin ne?"<<endl;
  cin>>x;
  cout<<"Memnun oldum "<<x<<endl;
  cout<<"Bu gun nasilsin?"<<endl;
  cin>>y;
  cout<<"Bunu duyduguma sevindim"<<endl;
  cout<<"Nelerden hoslanirsin?"<<endl;
  cin>>z;
  cout<<"demek "<<z<<" lerden hoslanırsın ";
  }
___________________________________________________________________________________________________________________

#include <iostream> 
using namespace std;
int main() {

int a=5;
int *ptr = &a;

cout<<"değiskenin adresi "<<&a<<endl;
cout<<"degiskenin adresi ama bu kez ptr "<<*ptr<<endl;
cout<<"degiskenin degeri "<<ptr<<endl;

*ptr=8;

cout<<"yeni deger "<<&a<<endl;
cout<<"yeni deger "<<*ptr<<endl;
cout<<"bu da yeni deger "<<ptr<<endl; 

  }

___________________________________________________________________________________________________________________

#include <iostream> 
using namespace std;
void bugday(int *ptr){
	*ptr = 20;
	cout<<"fok1 "<<*ptr<<endl;
	
}

int main() {
 int a= 10;
 cout<<"a degiskenin degeri "<<a<<endl;
 bugday(&a);
 cout<<"a degiskenin yeni degeri"<<a<<endl;

  }

___________________________________________________________________________________________________________________

#include <iostream> 
using namespace std;

int main() {
 int array[] = {1,2,3,4};
 
  cout<<array  <<endl;
  cout<<array+1<<endl;
  cout<<array+2<<endl;
  }

___________________________________________________________________________________________________________________
___________________________________________________________________________________________________________________

__
