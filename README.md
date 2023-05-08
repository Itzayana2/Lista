# Lista
public class Lista{
    Nodo primero;
    int indice;
    
    public Lista () {
        primero=null;
        indice=-1;
    }
    public void insertar (String dato){
        Nodo temp=new Nodo (dato);
        temp.next=primero;
        primero=temp;
        indice ++;
    
    }
    public void buscar(int indice) {
        Nodo temp=new Nodo( );
        Nodo n=primero;
        for(int i=0; (i<indice)&&(n!=null);i++){
            n=n.next;
            temp=n;
        }
        Sistem.out.println(temp.info);
    }
    public void visualizar () {
        Nodo n;
        n=primero;
        while(n!=null){
            System.out.primtln(n.info);
            n=n.next;
        }
    }
}
