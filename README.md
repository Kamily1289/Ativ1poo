public class Principal {
    public static void main(String[] args) {
        // Criação do objeto da classe Professor
        Professor professor1 = new Professor(101, "João da Silva", "Ciência da Computação");
        Professor professor2 = new Professor(102, "Maria Souza", "Engenharia Civil");

        // Invoca o método para imprimir os dados do primeiro professor
  System.out.println("--- Dados do Professor 1 ---");
        professor1.imprimirProfessor();

        // Invoca o método setter para alterar um atributo do segundo professor
  System.out.println("\n--- Dados do Professor 2 (antes da alteração) ---");
        professor2.imprimirProfessor();
        professor2.setNomeDepartamento("Arquitetura");

        // Invoca o método getter para obter um atributo e imprimir separadamente
  System.out.println("\n--- Dados do Professor 2 (após a alteração) ---");
  System.out.println("Novo Departamento: " + professor2.getNomeDepartamento());
        professor2.imprimirProfessor();
    }
}
