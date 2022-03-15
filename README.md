# Exercicios_Poo_Java_Faculdade
Q1
package lista1;

import java.util.Scanner;

public class q1 {
	public static void main(String[]ars){
		Scanner sc = new Scanner(System.in);
		int a ,b ,c, delta ;
		double x1,x2;
						
		System.out.println("Digite o valor de A: ");
		a = sc.nextInt();
		
		System.out.println("Digite o valor de B: ");
		b = sc.nextInt();
		
		System.out.println("Digite o valor de C: ");
		c = sc.nextInt();
		delta = ((b*b)-(4*a*c));
		x1 = 0;
		x2 = 0;		
		
		if(delta==0) {
			System.out.println("Há uma raiz real");
			x1=(-b)/(2*a);
			System.out.println("X! = " + x1);
		}
		if(delta > 0) {
			System.out.println("Existem duas raizes reais:");
			x1= ((-b + Math.sqrt(delta)) / (2*a));
			x2=((-b - Math.sqrt(delta)) / (2*a));
			System.out.println("x1 vale :" +x1);
			System.out.println("x2 vale :" +x2);
		} 
		else {
			System.out.println("Delta invalido! ");
		}
	}
}
==============================================================================

Q2
package lista1;

public class q2 {
	public static void main(String[]args) {
		boolean a=true;
		boolean b=true;
		boolean c=false;
		
		if(a==true) {
			System.out.println("comando1");
		}else {
			if(b==true) {
				if(c==true) {
					System.out.println("comando2");
				}else {
					System.out.println("comando3");
					System.out.println("comando4");
				}
			}
		System.out.println("comando5 "); 
	}
	System.out.println("comando6");
	}
}

A
B
C
resposta
V
V
F
Comando 1 e 6
F
V
V
Comando 2,5,6
F
V
V
Comando 2,5,6
F
F
V
Comando 5 e 6
N ha resposta
================================================================================

Q3

package lista1;

import java.util.Scanner;


	public class q3 {
	public static void main(String[]args){
	Scanner sc = new Scanner(System.in);
    
	double  h=0,r=0,  area_do_cilindro = 0;
	double  altura_do_cilindro =0,raio_do_cilindro =0;	 
	int calcular_quantidade_de_latas_de_tinta =0 ;	
	float custo=0;
		
	System.out.println("Digite o raio do clindro: ");
	r = sc.nextInt();
	System.out.println("Digite a altura do cilindro: ");
    	h = sc.nextInt();
	
	altura_do_cilindro = h;
	raio_do_cilindro = r;
	
	area_do_cilindro = 2*3.14*raio_do_cilindro*(altura_do_cilindro+raio_do_cilindro);
	calcular_quantidade_de_latas_de_tinta = (int) (area_do_cilindro/3.0);		
	System.out.println("A area do Cilindro é: " );
	System.out.format("%.2f", area_do_cilindro );	
		custo = calcular_quantidade_de_latas_de_tinta*50;		
	System.out.println("\nA quantidade de latas de tinta é: " );
	System.out.println( calcular_quantidade_de_latas_de_tinta );	
	System.out.println("\nO custo para pintar um tanque no formato cilíndrico é: " );
	System.out.println(   custo);
	  			}
		}
========================================================================================================	
Q4
package lista1;
import java.util.Scanner;
public class q4 {
public static void main(String[]args){
Scanner sc = new Scanner(System.in);
//Escreva uma classe que receba do usuário cinco diferentes números inteiros e exiba em ordem
//decrescente. Para isto utilize uma condicional encadeada.	
int n1,n2,n3,n4,n5, auxiliar=0 ;
		System.out.println("Digite o primeiro numero: ");
		n1 = sc.nextInt();		
		System.out.println("Digite o segundo numero: ");
		n2 = sc.nextInt();		
		System.out.println("Digite terceiro numero: ");
		n3 = sc.nextInt();		
		System.out.println("Digite o quarto numero: ");
		n4 = sc.nextInt();		
		System.out.println("Digite o quinto numero: ");
		n5 = sc.nextInt();		
		if (n1 > n2) {
            auxiliar = n1;
            n1 = n2;
            n2 = auxiliar;
        }
        if (n2 > n3) {
            auxiliar = n2;
            n2 = n3;
            n3 = auxiliar;
        }              
        if (n3 > n4) {
            auxiliar = n3;
            n3 = n4;
            n4 = auxiliar;
        }
        if (n4 > n5) {
            auxiliar = n4;
            n4 = n5;
            n5 = auxiliar;
        }
		System.out.println(" A ordem decrecente dos numeros são: "  + n5 +" " + n4 +" "+ n3 +" "+ n2 +" "+ n1);				
}
}

===============================================================================================================================
