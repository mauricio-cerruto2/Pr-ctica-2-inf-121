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
        linea.dibujaLinea(g); // Dibuja la línea
    }
}
    public toString() {
                return "Linea{del punto:" +p1+ "hasta el punto:" +p2+ "}";
		
	       }
	      public static void main(String[] args) {
		   
		
		    }
	

}
Codigo de la clase Linea en python:
class linea:
import matplotlib.pyplot as plt
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
                   
