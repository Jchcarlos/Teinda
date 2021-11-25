# Teinda
import javax.swing.JOptionPane;
public class Tienda_1 {

    public static void main(String[] args) {
        int Opcion, costo, TotalC = 0,TotalComp = 0, TotalTel = 0, TotalProd = 0, TotalDinero = 0;
        int TotalRef = 0, TotalX = 0, TotalR = 0;
        int IVA, ProdC = 0, ProdComp = 0, ProdTel = 0, ProdRef = 0, ProdX = 0, ProdR = 0;    //0.16
        int C = 0, C1 = 0, Com = 0, Com1 = 0, Tel = 0, Tel1 = 0, Ref = 0, Ref1 = 0, X = 0, X1 = 0, R = 0, R1 = 0;
        double Cel = 5.550,Compu = 9.000,Telv = 15.000,Refresco = 26,Xbox = 10.000,Ropa = 500;;
        String r;  
        
        JOptionPane.showMessageDialog(null,"Hola, muy buenos dias bienvenido a Tienda Carlitos :) ");
    

        do {
            Opcion = Integer.parseInt(JOptionPane.showInputDialog("Nuestra tienda cuneta con los siguientes pdroductos "
                + "\n 1 Celular $5,500"
                + "\n 2 Computadora $9,000"
                + "\n 3 Television $15,000"
                + "\n 4 Rrefresco $26"
                + "\n 5 Viaje $10,000"
                + "\n 6 Ropa $500"
                + "\n 7 Cantidad de productos vendidos"
                + "\n 8 Costo total de productos vendidos"
                + "\n9 Costo total de productos vendidos mas IVA"));

            switch (Opcion) {
                
                case 1:
                    
                    JOptionPane.showMessageDialog(null, "Seleccionaste el poducto Celular");
                    costo = Integer.parseInt(JOptionPane.showInputDialog("Selecciona donde quieres realizar la compra "
                            + "\n 1. Precio en tienda Celular $5,500 "
                            + "\n 2. Precio en linea IVA Celular 16% "));

                    if (costo == 1) {
                        
                        C += Cel;
                        ProdC++;
                        TotalProd += Cel;
                        TotalDinero += C;
                        
                    }
                    
                    if (costo == 2) {
                        
                        C1 += 5550 + (5550 * 0.16);
                        ProdC++;
                        TotalProd += ProdC;
                        TotalDinero += C1;
                        
                    }
                    
                    JOptionPane.showMessageDialog(null, "Costo del celular mas IVA "+C1);
                    
                    JOptionPane.showMessageDialog(null, "Gracias por su compra ");
                    
                    break;
                    
                case 2:
                        
                    JOptionPane.showMessageDialog(null, "Seleccionaste el poducto Computadora");
                    
                    costo = Integer.parseInt(JOptionPane.showInputDialog("Selecciona donde quieres realizar la compra "
                            + "\n 1. Precio en tienda Computadora $9,000 "
                            + "\n 2. Precio en linea IVA Computadora 16% "));

                    if (costo == 1) {
                        
                        TotalComp += Compu;
                        ProdComp++;
                        TotalProd += Compu;
                        TotalDinero += Com;
                        
                    }
                    
                    if (costo == 2) {
                        
                        Com1 += 9000 + (9000 * 0.16);
                        ProdComp++;
                        TotalProd += ProdComp;
                        TotalDinero += Com1;
                        
                    }
                    
                    JOptionPane.showMessageDialog(null, "Costo de la Computadora mas IVA "+Com1);

                    break;
                    
                case 3:
                    JOptionPane.showMessageDialog(null, "Seleccionaste el poducto Television ");
                    costo = Integer.parseInt(JOptionPane.showInputDialog("Selecciona donde quieres realizar la compra "
                            + "\n 1. Precio en tienda Television $15,000"
                            + "\n 2. Precio en linea IVA Television 16% "));

                    if (costo == 1) {
                        
                        TotalTel += Telv;
                        ProdTel++;
                        TotalProd += Telv;
                        TotalDinero += Tel;
                        
                    }
                    
                    if (costo == 2) {
                        
                        Tel1 += 15000 + (15000 * 0.16);
                        ProdTel++;
                        TotalProd += ProdTel;
                        TotalDinero += Tel1;
                        
                    }
                    
                    JOptionPane.showMessageDialog(null, "Costo del Television mas IVA "+Tel1);

                    break;
                    
                case 4:
                    JOptionPane.showMessageDialog(null, "Seleccionaste el poducto Rrefresco ");
                    costo = Integer.parseInt(JOptionPane.showInputDialog("Selecciona donde quieres realizar la compra "
                            + "\n 1. Precio en tienda Rrefresco $26 "
                            + "\n 2. Precio en linea IVA Celular 16% "));

                    if (costo == 1) {
                        
                        TotalRef += Refresco;
                        ProdC++;
                        TotalProd += Refresco;
                        TotalDinero += Ref;
                        
                    }
                    
                    if (costo == 2) {
                        
                        Ref1 += 26 + (26 * 0.16);
                        ProdRef++;
                        TotalProd += Refresco;
                        TotalDinero += Ref1;
                        
                    }
                    
                    JOptionPane.showMessageDialog(null, "Costo del refresco mas IVA "+Ref1);

                    break;
                    
                case 5:
                    
                    JOptionPane.showMessageDialog(null, "Seleccionaste el poducto Xbox ");
                    costo = Integer.parseInt(JOptionPane.showInputDialog("Selecciona donde quieres realizar la compra "
                            + "\n 1. Precio en tienda Xbox $10,000 "
                            + "\n 2. Precio en linea IVA Xbox 16% "));

                    if (costo == 1) {
                        
                        TotalX += Xbox;
                        ProdX++;
                        TotalProd += Xbox;
                        TotalDinero += X;
                        
                    }
                    
                    if (costo == 2) {
                        
                        X1 += 10000 + (10000 * 0.16);
                        ProdX++;
                        TotalProd += ProdX;
                        TotalDinero += X1;
                        
                    }
                    
                    JOptionPane.showMessageDialog(null, "Costo del Xbox mas IVA "+X1);

                    break;
                case 6:
                    
                    JOptionPane.showMessageDialog(null, "Seleccionaste el poducto Ropa ");
                    costo = Integer.parseInt(JOptionPane.showInputDialog("Selecciona donde quieres realizar la compra "
                            + "\n 1. Precio en tienda Ropa $500 "
                            + "\n 2. Precio en linea IVA 16% "));

                    if (costo == 1) {
                        
                        TotalR += Ropa;
                        ProdR++;
                        TotalProd += Ropa;
                        TotalDinero += R;
                        
                    }
                    
                    if (costo == 2) {
                        
                        R1 += 555 + (555 * 0.16);
                        ProdR++;
                        TotalProd += ProdR;
                        TotalDinero += R1;
                        
                    }
                    
                    JOptionPane.showMessageDialog(null, "Costo de la ropa mas IVA "+R1);

                    break;
                default:
                    JOptionPane.showMessageDialog(null, "No contamos con esta opcion una disculpa, intentalo mas tarde");

                            JOptionPane.showMessageDialog(null, " " + ProdR + "\n Total ropa $ " + R1);
  
            }

            r = JOptionPane.showInputDialog("Deseas agregar otro producto a su carrito SI/NO");
        } while (r.equalsIgnoreCase("Si") || r.equalsIgnoreCase("No"));

        JOptionPane.showMessageDialog(null, "Total de productos celulares " + ProdC + "\n Total por celulares $ " + C);
        JOptionPane.showMessageDialog(null, "Total de productos celulares mas IVA " + ProdC + "\n Total por celulares $ " + C1);
        JOptionPane.showMessageDialog(null, "Total de productos computadora " + ProdComp + "\n Total computadora $ " + Com);
        JOptionPane.showMessageDialog(null, "Total de productos computadora mas IVA " + ProdComp + "\n Total computadora $ " + Com1);
        JOptionPane.showMessageDialog(null, "Total de productos television " + ProdTel + "\n Tota television $ " + Tel);
        JOptionPane.showMessageDialog(null, "Total de productos television mas IVA " + ProdTel + "\n Tota television $ " + Tel1);
        JOptionPane.showMessageDialog(null, "Total de productos refresco " + ProdRef + "\n Total refresco $ " + Ref);
        JOptionPane.showMessageDialog(null, "Total de productos refresco mas IVA " + ProdRef + "\n Total refresco $ " + Ref1);
        JOptionPane.showMessageDialog(null, "Total de productos Xbox " + ProdX + "\n Total  Xbox $ " + X);
        JOptionPane.showMessageDialog(null, "Total de productos Xbox mas IVA " + ProdX + "\n Total  Xbox $ " + X1);
        JOptionPane.showMessageDialog(null, "Total de productos ropa " + ProdR + "\n Total ropa$ " + R);
        JOptionPane.showMessageDialog(null, "Total de productos ropa mas IVA " + ProdR + "\n Total ropa$ " + R1);
        JOptionPane.showMessageDialog(null, "Cuantos de los productos tienen un precio superior al promedio de compra " + ProdTel + "\n Total $ " + Tel);
        JOptionPane.showMessageDialog(null, "Total de boletos vendidos " + TotalProd);
        JOptionPane.showMessageDialog(null, "Costo total de boletos vendidos $ " + TotalDinero);
    }
}
