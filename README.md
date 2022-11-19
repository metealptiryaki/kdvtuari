import java.util.Scanner;
public class Kdvtutari {
	public static void main(String[] args) {
		/*Java ile kullanıcıdan alınan para değerinin KDV'li fiyatını ve KDV tutarını hesaplayıp ekrana bastıran programı yazın.
		(Not : KDV tutarını 18% olarak alın)
		KDV'siz Fiyat = 10;
		KDV'li Fiyat = 11.8;
		KDV tutarı = 1.8;
		 * 
		 */
		//%18 olarak verdiği yeri 0.18 olarak dönüştürmen gerek.
		//Double ile tanımlama sebebimiz girilecek sayıların virgüllü olması.
		double tutar,kdvOran = 0.18,kdvTutar,kdvliTutar;
		Scanner k = new Scanner(System.in);
		System.out.print("Ucret tutarini giriniz :");
		tutar = k.nextDouble();
		kdvTutar = tutar*kdvOran;
		kdvliTutar = kdvTutar+tutar;
		
		System.out.println("KDV'siz Tutar : "+tutar);
		System.out.println("KDV Orani: "+kdvOran);
		System.out.println("KDV Tutari10 :"+kdvTutar);
		System.out.println("KDV'li Tutar :"+kdvliTutar);
		
		
	}

}
