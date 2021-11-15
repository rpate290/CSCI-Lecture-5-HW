# CSCI-Lecture-5-HW
package lecture5Hw;

public class Hw5 {

class payCalculator{
	double payRate;
	double hours;
	double computePay(double pay, double hours) {
		return hours*pay;
	}
class regularPay extends payCalculator{
	regularPay(double i,double n){
		 payRate= i;
	     hours= n;
		
	}

	
}
class hazardPay extends payCalculator{
	double computePay(double pay, double hours) {
		return hours*pay*1.5;
	}
class discountPolicy{
	double itemCount;
	double itemCost;
	double computeDiscount(double count, double itemcost) {
	return count*itemcost/2;
}
}
class bulkDiscount extends discountPolicy{
	int minimum;
	double discount;
	double total;
	bulkDiscount(int m, double p){
	minimum=m;
	discount=p;
	double filler = 0;
		 if (itemCount>m) 
		 	total=computeDiscount(itemCount, itemCost);
		 else 
			 filler=computeDiscount(itemCount, itemCost);
		 	total=filler*2;
		 	
		 
}}
