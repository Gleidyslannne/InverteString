# InverteString
package com.mycompany.invertestring;


public class InverteString {

    
    
     public static void main(String[] args) {
        // String a ser invertida
        String inputString = "Olá, mundo!"; // Você pode alterar esta string conforme desejado
        
        // Chama o método para inverter a string
        String invertedString = inverteString(inputString);
        
        // Exibe a string invertida
        System.out.println("A string original é: " + inputString);
        System.out.println("A string invertida é: " + invertedString);
    }
    
    // Método para inverter uma string
    public static String inverteString(String str) {
        // Converte a string para um array de caracteres
        char[] charArray = str.toCharArray();
        
        // Inicializa um StringBuilder para armazenar a string invertida
        StringBuilder inverted = new StringBuilder();
        
        // Itera sobre os caracteres da string de trás para frente e os adiciona ao StringBuilder
        for (int i = charArray.length - 1; i >= 0; i--) {
            inverted.append(charArray[i]);
        }
        
        // Converte o StringBuilder de volta para uma string e a retorna
        return inverted.toString();
    }
}
