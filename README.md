# Membuat File PDF dengan java

1. create java class

import java.io.IOException;  
import org.apache.pdfbox.pdmodel.PDDocument; 
import org.apache.pdfbox.pdmodel.PDPage;  

public class CreatingEmptyPdf { 
   public static void main(String args[]) throws IOException { 
      
      //Creating PDF document object 
      PDDocument document = new PDDocument();     
     
      //Add an empty page to it 
      document.addPage(new PDPage()); 
     
      //Saving the document 
      document.save("D:/javafundamental/BlankPdf.pdf"); 
      System.out.println("PDF created");  
      
      //Closing the document  
      document.close(); 
   }  
}

<strong>2. Download libary pdfbox yang format jar</strong><br/>
https://pdfbox.apache.org/download.html

<strong>3. compile class java</strong><br/>
javac -cp .;pdfbox-app-2.0.9.jar CreatingEmptyPdf.java

<strong>4. Jalankan program</strong><br/>
java -cp .;pdfbox-app-2.0.9.jar CreatingEmptyPdf<br/><br/>

note: hasil download dan file class java di tempatkan di path yang sama
