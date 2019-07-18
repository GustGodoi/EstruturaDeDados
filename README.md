# EstruturaDeDados


package estruturadados;

import java.util.ArrayList;

public class EstruturaDados {

    public static void main(String[] args) {
    
        //CRIAMOS A LISTA DINÂMICA
        ArrayList<Integer> lista = new ArrayList();
        lista.add(10);
        lista.add(9);
        lista.add(58);
        lista.add(42);
        lista.add(1);
        lista.add(6);
        lista.add(2);
        
        //PERCORRE A LISTA E IMPRIME
        int aux = 0;
        for (int i = 0; i < lista.size(); i++) {
            aux = lista.get(i);
            System.out.println(aux);
        }
        
        //ADICIONA MAIS ITENS A LISTA
        lista.add(90);
        lista.add(100);
        //REMOVE ESTE ITEM DA LISTA
        lista.remove(0);
        
        System.out.println("---------------");
        //PERCORRE A LISTA (PELAS MUDANÇAS) E IMPRIME
        System.out.println("ArrayList Editado:");
        for (int i = 0; i < lista.size(); i++) {
            aux = lista.get(i);
            System.out.println(aux);
        }
        
        //CHAMA O PRIMEIRO ITEM DA LISTA
        System.out.println("---------------");
        System.out.println("Primeiro item da lista:");
        System.out.println(lista.get(0));
        
        //CHAMA O ÚLTIMO ITEM DA LISTA
        System.out.println("---------------");
        int ultimoIndice = (lista.size() -1);
        System.out.println("ultimo item da lista:");
        System.out.println(lista.get(ultimoIndice));
                
    }
    
}
