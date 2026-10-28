package edu.monmouth.campusvehicle;

public class CampusVehicle {

	// Q1: Add an additional attribute (color) from the UML diagram.
	private String id;
	private String location;
	private boolean available;
	private Color color;
	//private static final String UNKNOWN = "unknown";
	
	//Q5: Default constructor for backwards compatibility.
	//Uses construtor delegation ('this(...)') to show the 4-argument constructor.
	public CampusVehicle() {
		this("vehicle1", "main campus", true, Color.UNKNOWN);
	}
	
	public CampusVehicle(String id, String location, boolean available) {
		this(id, location, available, Color.UNKNOWN);
	}
	
	//Q5: 3-argument constructor for backwards compatibility.
	//Sets color to Color.UNKNOWN by delegating to the 4-argument constructor.
	public CampusVehicle(String id, String location, boolean available, Color color) {
		setId(id);
		setLocation(location);
		setAvailable(available);
		setColor(color);
	}
	
	//Accessor for id.
	public String getId() {
		return id;
	}
	
	//Q6-7: id must have minimum length 6, maximum length 18, and be stored as lowercase.
	public void setId(String id) {
		if (id != null && id.length() >= 6 && id.length() <= 18) {
			this.id = id.toLowerCase();
		} else {
			System.out.println("Error: ID must be between 6 and 18 characters.");
		}
	}
	
	//Accessor for location.
	public String getLocation() {
		return location;
	}
	
	//Q7: Location must always be stored as lowercase.
	public void setLocation(String location) {
		if (location != null) {
			this.location = location.toLowerCase();
		}
	}
	
	//Accessor for availablitiy.
	public boolean isAvailable() {
		return available;
	}
	
	//Mutator for availablitiy.
	public void setAvailable(boolean available) {
		this.available = available;
	}
	
	//Q3: Mutator for the color attribute.
	public void setColor(Color color) {
		this.color = color;
	}
	
	//Q3: Accessor for the color attribute.
	public Color getColor() {
		return color;
	}
	
	//Standard vehicle methods from UML diagram.
	public void checkOut() {
		if (available) {
			available = false;
		}
	}
	
	public void returnVehicle() {
		available = true;
	}
	
}
