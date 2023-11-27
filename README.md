# IMPACTO_ECOLOGICO
//Clase Edificio
 Class Edificio{
   private final int numeroPisos;
   private final string direccion;

   public Edificio(final int numeroPisos, final string direccion){
   this.numeroPisos = numeroPisos;
    this.direccion = direccion;
  }
  plubic void mostrarInformacion(){
    System.out.println("Edificio de " + numeroPisos + " pisos ubicado en " + direccion);
  }
}
//Clase Auto
class Auto{
  private string marca;
  private final string modelo;

  public Auto(final String marca, final String modelo){

    this.modelo = modelo;
  }
   public void conducir(){
     System.out.println("Conduciendo el auto " + marca + " " + modelo);
  }        
}
//Clase Bicicleta
class Bicicleta{
 private final String tipo;
  private final int numeroEngranajes;

  public Bicicleta(final String tipo, final int numeroEngranajes){
    this.tipo = tipo;
    this.numeroEngranajes = numeroEngranajes;
  }

  public void pedalear(){
    System.out.println("Pedaleando en una bicicleta" + tipo + "con " + numeroEngranajes + " engranajes");
  }
}
//Ejemplo de uso
public class Main {
  public static void main(final String[] aegs){
    final Edificio edificio = new Edificio(10, "Calle Principal");edificio.mostrarInformacion();

    final Auto auto = new Auto("Toyota","Camry");auto.conducir();

    final Bicicleta bicicleta = new Bicicleta("Montaña", 21);bicicleta.pedalear();
  }
     plublic @Override
public String toString() {
	return "Main []";
}
	interface ImpactoEcologico{
   int obtenerImpactoEcologico();
 }
  public class Vehiculo implemets ImpactoEcologico{
    //Otros atributos y metodos de la clase Vehiculo

    @Override
      public double obtenerImpactoEcologico(){
      // Cálculo del impacto ecologico del vehiculo
      //...
      // Retorna el valor del impacto ecologico calculado
      return impactoEcologico;
      }
  }
  public interface ImpactoEcologico{
    double obternerImpactoEcologico();
  }
  public class Edificio implements ImpactoEcologico{
    private double emisionesCO2; // Emisiones de CO2 especificas del edificio

    // Constructor y otros metodos de la clase Edificio
    @Override
    public double obtenerImpactoEcologico(){
      // Logica para calcular el impacto ecologico del edificio
      return emisionesCO2;
    }
  }
 public class Auto implements ImpactoEcologico{
   private double emisionesCO2; //Emisiones de CO2 especificas del auto

   // Construtor y otros metodos de la clase Auto
   
    @Override
   public double obtenerImpactoEcologico(){
     // Logica para calcular el impacto ecologico del carbono del auto
     return emisionesCO2;
   }
 }
  public class Bicicleta implements   ImpactoEcologico {
    private double emisionesCO2; // Emisiones de CO2 especificas de la bicicleta
    // Constructor y otros metodos de la clase Bicicleta
    return emisionesCO2;
      
  }
 
import java.util.ArrayList;

  public static void main(String[] args){
    ArrayList<ImpactoEcologico> objetosImpacto = new ArrayList< >();

    // Crear objetos de cada clase y agregar las referencias al ArraList
    Edificio edificio = new Edificio("Edificio A");
    objetosImpacto.add(edificio);

    Auto auto = new Auto("Auto B");
    objetosImpacto.add(auto);

    Bicicleta bicicleta = new Bicicleta("Bicicleta C");
     objetosImpacto.add(bicicleta);
    
    // Iterar el ArrayList e invocar polimorfisicamente el metodo obtenerImpactoEcologico()
    for (ImpactoEcologico objeto: objetoImpacto){
      double impactoEcol = objeto.obtenerImpactoEcologico();
      String identificacion = objeto.obtenerInformacionIdentificasion();
      System.out.println("Informacion de identificacion:");
      System.out.println(identificacion);
      System.out.println("Impacto ecologico del carbono: " + impactoEcol);
      System.out.println();
      
    }
  }
}

public interface ImpactoEcologico{
 
