public class persona {
    protected String nombre;
    protected int edad;

    public persona(String nombre, int edad) {
        this.nombre = nombre;
        this.edad = edad;
    }

    public void yourself() {
        System.out.println("Hola, soy " + nombre + " y tengo " + edad + " años.");
 }
     }
public class Estudiante extends persona {
    private String matricula;
    private String carrera;

    public Estudiante(String nombre, int edad, String matricula, String carrera) {
        super(nombre, edad);
        this.matricula = matricula;
        this.carrera = carrera;
    }

    @Override
    public void yourself() {
        super.yourself();
        System.out.println("Soy estudiante de la carrera: " + carrera + " con matrícula: " + matricula);
    }
}
public class profesor extends persona {
    private String especialidad;
    private String grupoAsignado;

    public profesor(String nombre, int edad, String especialidad, String grupoAsignado) {
        super(nombre, edad);
        this.especialidad = especialidad;
        this.grupoAsignado = grupoAsignado;
    }

    @Override
    public void yourself() {
        super.yourself();
        System.out.println("Soy profesor de " + especialidad + " y tengo a cargo el grupo: " + grupoAsignado);
    }
}
public class main {
    public static void main(String[] args) {
        Estudiante estudiante = new Estudiante("Ana", 20, "A12345", "Ingeniería");
        profesor profesor = new profesor("Carlos", 45, "Matemáticas", "3A");

        estudiante.yourself();
        System.out.println("------------------");
        profesor.yourself();
    }
}# replicacion_poo-to-fork
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
