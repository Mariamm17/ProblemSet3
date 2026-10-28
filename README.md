# ProblemSet3

package edu.monmouth.problemSet3;

import edu.monmouth.campusvehicle.CampusVehicle;
import edu.monmouth.campusvehicle.Color;

public class ProblemSet3 {

	public static void main(String[] args) {
		
		//Q8a: Placed in package edu.monmouth.problemSet3.
		
		System.out.println("--- Regression Testing Default Constructor ---");
		
		//Q8b: Create a Campus Vehicle object using thedefault constructor.
		CampusVehicle vehicle1 = new CampusVehicle();
		
		//Q8c: Retrieve and print all attributes (Regression Testing).
		System.out.println("Default constructor values:");
		System.out.println("ID: " + vehicle1.getId());
		System.out.println("Location: " + vehicle1.getLocation());
		System.out.println("Available: " + vehicle1.isAvailable());
		System.out.println("Color: " + vehicle1.getColor());
		
		System.out.println("\n--- Using Mutators on Vehicle 1 ---");

		//Q8d: Using the four mutators, set attributes to valid values.
		vehicle1.setId("monmouth123");
		vehicle1.setLocation("Library Lot");
		vehicle1.setAvailable(false);
		vehicle1.setColor(Color.BLUE);
		
		//Q8e: Retrieve and print all attributes for this object.
		System.out.println("Updated vehicle1 values:");
		System.out.println("ID: " + vehicle1.getId());
		System.out.println("Location: " + vehicle1.getLocation());
		System.out.println("Available: " + vehicle1.isAvailable());
		System.out.println("Color: " + vehicle1.getColor());
		
		System.out.println("\n--- Creating Vehicle with All 4 Attributes ---");
		
		//Q8f: Create another object using the 4-argument constructor.
		CampusVehicle vehicle2 = new CampusVehicle("hawkshuttle", "Student Center", true, Color.RED);
		
		System.out.println("ID: " + vehicle2.getId());
		System.out.println("Location: " + vehicle2.getLocation());
		System.out.println("Available: " + vehicle2.isAvailable());
		System.out.println("Color: " + vehicle2.getColor());
		
		//Q8g: Retrieve and print all attributes immediately.
		System.out.println("\n--- Changing Color on Vehicle 2 ---");
		
		//Q8h: Using a mutator method, change this object's color.
		vehicle2.setColor(Color.GREEN);
		
		//Q8i: Retrieve and print all attributes for this object.
		System.out.println("Modified vehicle2 values:");
		System.out.println("ID: " + vehicle2.getId());
		System.out.println("Location: " + vehicle2.getLocation());
		System.out.println("Available: " + vehicle2.isAvailable());
		System.out.println("Color: " + vehicle2.getColor());
		
		System.out.println("\n--- Creating More Vehicles to Verify ---");
		
		//Q8j: System.out.println("\n--- Creating More Vehicles to Verify ---");.
		CampusVehicle vehicle3 = new CampusVehicle(" scoutsVan", " Science Building", false, Color.BLACK);
		CampusVehicle vehicle4 = new CampusVehicle(" campusCar99", " West Campus", true); // 3-arg constructor
		
		System.out.println("Vehicle 3 -> ID: " + vehicle3.getId() + ", Location: " + vehicle3.getLocation() + ", Available: " + vehicle3.isAvailable() + ", Color: " + vehicle3.getColor());
		System.out.println("Vehicle 4 -> ID: " + vehicle4.getId() + ", Location: " + vehicle4.getLocation() + ", Available: " + vehicle4.isAvailable() + ", Color: " + vehicle4.getColor());
	}
}
