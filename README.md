class Figura

{

Figura(float ax=0, float ay = 0 )

void Pisz();

void Przesun(float dx, float dy )

private:

float x, y;
};
class Okrag public Figura

{

public:

Okrag(float ar=1, float ax=0, float ay=0);

void Pisz();

float Obwod();

private:

float r;
};Okrag: Okrag(float ar, float ax, float ay) Figura(ax, ay)
{
if (ar>0) r = ar 
else r = 1
}
void Okrag::Pisz()

{

Figura:: Pisz();

cout <<" r = "<<<r<<<endl;

}
int main ()
{

Okrag o(10)

cout<<"Polozenie i promien okregu:"<<endl; o.Pisz();

cout<<"Obwod: "<<o.Obwod()<<endl;

o. Przesun (2, 3)

cout<<"Dane okregu po przesunieciu:"<<endl;

o. Pisz();

return 0;
}
