mi# Pr-ctica-2-inf-121
Codigo de la clases Linea en Java:
package prac;
import javax.swing.*;
import java.awt.*;
public class Linea{
	       public  punto punto1;
	       public  punto punto2;
	       public Linea (Punto punto1 , Punto punto2) {
	               	punto1 = punto1;
	               	punto2  = punto2;
	       }
    public void dibujaLinea(Graphics g) {
        g.drawLine(punto1.x, punto1.y, punto2.x, punto2.y);
    }
}

class DibujoPanel extends JPanel {
    private Linea linea;
    public DibujoPanel(Linea linea) {
        this.linea = linea;
    }
    protected void paintComponent(Graphics g) {
        super.paintComponent(g);
        linea.dibujaLinea(g);
    }
}
    public toString() {
                return "Linea{del punto:" +p1+ "hasta el punto:" +p2+ "}";		
	       }
public static void main(String[] args) {		
		    }
	

}
Codigo de la clase Linea en python:
import matplotlib.pyplot as plt
class linea:
         def_init_(self, p1 ,p2):
                 self.p1= p1
                 self.p2=p2
         def_str_(self):
                 return str(self.p1)+"----"+(self.p2)
         def dibujaLinea(self)
                 x_coords = [self.punto1.x, self.punto2.x]
        y_coords = [self.punto1.y, self.punto2.y]
                        plt.plot(x_coords, y_coords, marker='o')
                 plt.xlabel('Eje X')
                 plt.ylabel('Eje Y')
                 plt.title('Línea entre dos puntos')
                 plt.grid(True)
                 plt.show()


punto1 = Punto(1, 2)
punto2 = Punto(4, 6)
linea = Linea(punto1, punto2)
linea.dibujaLinea()



Codigo de la clase Círculo en Java:


package prac;
import javax.swing.*;
import java.awt.*;
public class Circulo{
	       public  punto  centro;
	       public  float   radio;
	       public Punto(punto centro , float radio) {
	               	centro = centro;
	               	radio = radio;
	       }
       	public toString() {
                return "Circulo{con centro en:" +centro+ "y radio:"                                                    +radio+ "}";		
	       }
public void dibujaCirculo(Graphics g) {
        g.drawOval(centro.x - radio, centro.y - radio, 2 * radio, 2 * radio);
    }
}

class DibujoPanel extends JPanel {
    private Circulo circulo;
    public DibujoPanel(Circulo circulo) {
        this.circulo = circulo;
    }
    protected void paintComponent(Graphics g) {
        super.paintComponent(g);
        circulo.dibujaCirculo(g); 
    }
}
public toString() {
                return "Circulo{con centro en:" +c+ "y radio:"                                                    +r+"}";		
	       }
public class Main {
    public static void main(String[] args) {
    }
}


Codigo de la clase en Python:

import matplotlib.pyplot as plt
clases Circulo:
         def_init_(self, c1 ,r1):
                 self.c1= c1
                 self.r1=r1
         def_str_(self):
                 return str(self.c1)+"----"+(self.r1)
         def dibujaCirculo(self):
                 fig, ax = plt.subplots()
            circulo = plt.Circle((self.centro.x, self.centro.y), self.radio, color='blue', fill=False)
        ax.add_patch(circulo)
        ax.set_xlim(self.centro.x - self.radio - 10, self.centro.x + self.radio + 10)
        ax.set_ylim(self.centro.y - self.radio - 10, self.centro.y + self.radio + 10)
        ax.set_aspect('equal', adjustable='box')
        plt.xlabel('Eje X')
        plt.ylabel('Eje Y')
        plt.title('Círculo')
        plt.grid(True)
        plt.show()



centro = Punto(150, 150)
circulo = Circulo(centro, 100)
circulo.dibujaCirculo()
Print(c1)


	       
                   
