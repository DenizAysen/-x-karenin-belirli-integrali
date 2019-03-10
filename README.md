# -x-karenin-belirli-integrali

import java.util.Scanner;

import java.util.Locale;

public class xkareninbelirliintegrali {

	public static void main(String[] args) {
		
		
		Scanner sn= new Scanner(System.in);
		sn.useLocale(Locale.US);
		double altdeger,üstdeger;
		double h=0.0001;
		System.out.print("Altdeğeri giriniz:");
		altdeger=sn.nextDouble();
		System.out.print("\nÜstdeğeri giriniz:");
		üstdeger=sn.nextDouble();
		double alan=0.00;
		
		while(altdeger<=üstdeger) {
			alan+=h*Math.pow(altdeger,2);
			altdeger+=h;
			}
		
		
		System.out.println("Belirli integralin sonucu:"+alan);
	}

}
