# Construtores com Sobrecarga;
import javax.swing.*;

public class Aula13 {
    String nome;
    String endereco;
    String email;
    int cpf;

    public Aula13(String nome, String email){
        this.nome = nome;
        this.email = email;
        JOptionPane.showMessageDialog(null,"Nome: "+this.nome+"\nEmail: "+this.email);
    }

    public Aula13(String nome, String email, String endereco){
        this.nome = nome;
        this.email = email;
        this.endereco = endereco;
        JOptionPane.showMessageDialog(null,"Nome: "+this.nome+"\nEmail: "+this.email+"\nEndereço: "+this.endereco);
    }

    public Aula13(String nome, String email, String endereco, int cpf){
        this.nome = nome;
        this.email = email;
        this.endereco = endereco;
        this.cpf = cpf;
        JOptionPane.showMessageDialog(null,"Nome: "+this.nome+"\nEmail: "+this.email+"\nEndereço: "
                +this.endereco+"\nCPF: "+this.cpf);
    }

    public static void main(String[] args){
        Aula13 construtor1 = new Aula13("Adriano","adriano@hotmail.com");
        Aula13 construtor2 = new Aula13("Brasil","Brasil@hotmail.com","Brasília - DF");
        Aula13 construtor3 = new Aula13("Iverson", "iversonfreitas@hotmail.com","Cidade Ocidental - GO",
                00000);
    }
}
