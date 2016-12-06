# Horarioescolar
horario para introducir una materia 
//Creamos una cola
import java.util.ArrayList;

public class yourmonismypich extends ArrayList {
	
 public void insertar(Object dato) {
	      if (dato!=null){
	    	  this.add(dato);
	      }
	    
	        else
	        {
	        System.out.println("introduce diferente a null");  
	        }
	    }
	    
	    
 public Object cima(){
			Object datoAuxiliar=null;
			if(this.size()>0){
				datoAuxiliar=this.get(this.size()-1);
			}
			return datoAuxiliar;
	    	
	    }
	    
	    
	    public void desapilar(){
	    	if(size()>0){
	    		this.remove(this.size()-1);
	    	}}
	          
		        
		        
		        
	    }
      // despues hacemos el main
import java.util.Scanner;
	public class supercometin {
		public static void main(String[] ar) {
    Scanner sc= new Scanner(System.in);
   Object  dias;
   Object materias;

   yourmonismypich pilax=new yourmonismypich();
   
    
    for ( int i=0; i<5; i++){
    	System.out.println("Introduce tu dia");
    	dias=sc.next();
    	pilax.insertar(dias);
    }
    yourmonismypich pilax1=new yourmonismypich();
   
    for ( int i=0; i<5; i++){
    	System.out.println("Introduce tu materia");
    	materias=sc.next();
    	pilax1.insertar(materias);
   
    }
    System.out.println("DIAS:"+"         MATERIAS      ");
    for ( int i=0; i<5; i++){
    	System.out.print("\n"+pilax.cima()+"          "+pilax1.cima()) ;
    	
    	pilax.desapilar();
    	pilax1.desapilar();
    }
    	
	    
	        		        		        }
    
}
      
