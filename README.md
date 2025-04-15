# replicacion_poo-to-fork
pracitca fork

    
    
public class Estudiante extends Persona{
    String Matricula;
    String Carrera;

    public Estudiante(String Nombre,int Edad, String Matricula, String Carrera) {
        super(Nombre,Edad);
        this.Matricula = Matricula;
        this.Carrera = Carrera;
    }
     public void mostrarDato(){
         System.out.println("Nombre"+getNombre()+"Edad"+getEdad()+"Matricula"+Matricula+"Carrera"+Carrera);

   }     

    public class Profesor extends Persona {
    
    String Especialidad;
    String Grupo_asignado;

    public Profesor( String Nombre, int Edad,String Especialidad, String Grupo_asignado) {
        super(Nombre, Edad);
        this.Especialidad = Especialidad;
        this.Grupo_asignado = Grupo_asignado;
    }
     public void mostrarDato1(){
         System.out.println("Nombre"+getNombre()+"Edad"+getEdad()+"Especialidad"+Especialidad+"Grupo asignado"+Grupo_asignado);

   }    

    public class Persona {
    String Nombre;
    int Edad;

        public Persona(String Nombre, int Edad) {
        this.Nombre = Nombre;
        this.Edad = Edad;
    }

    public String getNombre() {
        return Nombre;
    }

    public int getEdad() {
        return Edad;
    }
