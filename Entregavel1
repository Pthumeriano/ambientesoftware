import java.util.Scanner;

class Main {

  public static boolean EhPrimo(int numero){

    if(numero == 1){return false;}

    for(int i=numero-1; i != 1; i--){
      if(numero % i == 0){
        return false;
      }
    }

    return true;
  }

  public static int somatorio(int numero){
    
    int resultado = 0;
    for(int i = numero; i > 0; i--){
      resultado += i;
    }

    return resultado;
    
  }

  public static int fibonacci(int numero){
    
    if(numero<=2){
      return 1;
    }
    
    return fibonacci(numero - 1) + fibonacci(numero - 2);
  }

  public static int mdc(int a, int b){
    int maior = b;
    if(a > b){maior = a;}

    for(int i=maior-1; i>1; i--){
      if((a%i == 0) && (b%i == 0)){
        return i;
      }
    }

    return 0;
    
  }

  public static int dividir(int arr[], int inicio, int fim){
    int pivo = arr[fim];
    int i = (inicio-1);
    for (int j=inicio; j<fim; j++){
      
    if (arr[j] <= pivo){
      i++; 
      
      int temp = arr[i];
      arr[i] = arr[j];
      arr[j] = temp;
    }
  }

  int temp = arr[i+1];
  arr[i+1] = arr[fim];
  arr[fim] = temp;
  return i+1;
}

  public static void quicksort(int arr[], int inicio, int fim){
    if(inicio < fim){
      int d = dividir(arr, inicio, fim);
      quicksort(arr, inicio, d-1);
      quicksort(arr, d+1, fim);
    }
  }

  public static int contagem(){
    
    System.out.print("Digite a quantidade de valores:  ");
    int n = new Scanner(System.in).nextInt();
    Float valores[] = new Float[n];
    
    for(int i=1; i<=n; i++){
      System.out.println("Digite o valor " + i);
      valores[i-1] = new Scanner(System.in).nextFloat();
    }
    
    int contador = 0;
    for(int i=0; i<valores.length; i++){
      if((valores[i] - valores[i].intValue()) == 0){
        contador++;
      }
    }
    return contador;
  }

  
  
  public static void main(String[] args) {
    
    System.out.println("Eh primo ou naum " + EhPrimo(5));
    System.out.println("Somatorio: " + somatorio(5));
    System.out.println("Fibonacci: " + fibonacci(6));
    System.out.println("MDC: " + mdc(400,320));
    System.out.println("");
    System.out.println("Valores inteiros: " + contagem());
    
    int arr[] = {1,2,0,5,4,9,3};
    quicksort(arr, 0, arr.length-1);

    for(int i=0; i<arr.length;i++){
      System.out.print(arr[i] + "  ");
    }
    
  }
}
