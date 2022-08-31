package test2;

import test2.DTO.Auto;
import test2.DTO.Vehiculo;

public class Main {

    public static void main(String[] args) {

        Vehiculo miVehiculo = new Vehiculo();
        
    
    miVehiculo.setMarca("Toyota");
    miVehiculo.setModelo("Yaris");
    miVehiculo.setPatente("Patente");
    
        System.out.println(miVehiculo.getMarca()
                +" "+miVehiculo.getModelo()
                +" "+miVehiculo.getPatente()
         );
         Auto miAuto = new Auto();
         miAuto.setCantidadPuertas(5);
         miAuto.setModelo("Susuki");
         miAuto.setModelo("swift");
         
        
        
        System.out.println(miAuto.getCantidadPuertas());
    }
              
    }
package test2.DTO;

public class Vehiculo {
    private String Marca;
    private  String Modelo;
    private  String Patente;
    private int CantidadRuedas;

    
    public Vehiculo(){
        this.Marca = "Chevrolet";
        this.Modelo = "Camaro";
        this.Patente = "Sin Patente";
        this.CantidadRuedas = 4;
        
    }
    public String getMarca(){
        return this.Marca;
        }
    public String getModelo(){
        return this.Modelo;
    }
    public String getPatente(){
        return this.Patente;
    }
    public int getCantidadRuedas(){
        return this.CantidadRuedas;
    }
    
    public void setMarca(String Marca){
        this.Marca = Marca;
        
    }
    public void setModelo(String Modelo){
        this.Modelo = Modelo;
    }
    public void setPatente(String Patente){
        this.Patente = Patente;
      
    }
   public void setCantidadRuedas(int CantidadRuedas){
       this.CantidadRuedas = CantidadRuedas;
   }
    
}

package test2.DTO;

public class Auto extends Vehiculo{
    private int CantidadPuertas;

    public int getCantidadPuertas() {
        return CantidadPuertas;
    }

    public void setCantidadPuertas(int CantidadPuertas) {
        this.CantidadPuertas = CantidadPuertas;
    }

   
    
    
    
}
