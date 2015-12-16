import java.awt.event.ActionEvent;				
import java.awt.event.ActionListener;
import javax.swing.JButton;
import javax.swing.JFrame;
import javax.swing.JPanel;
import javax.swing.JTextField;
import javax.swing.JLabel;
import java.awt.GridBagLayout;
import java.awt.GridBagConstraints;
import java.awt.Insets;
import javax.swing.JOptionPane;
// import all the packages that have to be used

public class Mark_O_ConnorA1 extends JFrame implements ActionListener{
	JButton button;
	JTextField myField;
	JTextField myField2;
	String myString;
	float sum;
	
	public Mark_O_ConnorA1(){
		setSize(300, 300); // setting the size of my window
		setVisible(true);  // setting it to visible so it can be seen		
		JTextField newTitle = new JTextField("Flops to Gflops Converter"); // creating a new title called Flops to GFlops Converter
		this.setTitle(newTitle.getText()); // setting the title
		JPanel panel = new JPanel(); // create a new panel
		this.add(panel); // add the panel to the frame
		GridBagLayout myLayout = new GridBagLayout(); //creating a new GridBagLayout
		panel.setLayout(myLayout); // set panel's layout to the GridBagLayout
		GridBagConstraints c = new GridBagConstraints();
		
		JLabel jLabel = new JLabel("Enter Flops:"); // create new JLabel called jLabel
		c.gridx = 0; 
		c.gridy = 0;
		c.insets = new Insets(10,10,10,10);
		panel.add(jLabel, c); // adding jLabel to the panel
	
		myField = new JTextField(15); //create a new textField 
		c.gridx = 1;
		c.gridy = 0;
	
		panel.add(myField, c); // adding myField to the panel
		
		JLabel jLabel1 = new JLabel("GigaFlops:");
		c.gridx = 0;
		c.gridy = 1;
		c.insets = new Insets(0,10,10,20);
		panel.add(jLabel1, c); // adding jLabel1 to the panel
		
		myField2 = new JTextField(15); // create my second textField
		c.gridx = 1;
		c.gridy = 1;
		c.insets = new Insets(10,10,20,10);
	
		panel.add(myField2, c);
		
		JButton button1 = new JButton("Convert!"); // create my new button called button which will be convert.
		c.gridx = 1;
		c.gridy =2;
		
		panel.add(button1, c); //add the button to the panel
		button1.addActionListener(this); // give the button an actionListener
			
		}
		public static void main(String [] args){
			new Mark_O_ConnorA1(); // calling my method Mark_O_ConnorA1 in my main method 
		
		}
	
		public void actionPerformed (ActionEvent e){
			try{
				
				float sum = (float)((Float.parseFloat(myField.getText()))/1000000000L); // parsing my sum and doing the conversion 
				if(sum <0){
					JOptionPane.showMessageDialog(null,"Please input a positive number"); //show meessage dialog if a negative number is entered
				}
				else if(sum == sum)
				myField2.setText(Float.toString (sum));	
				
		//		else if(sum < 0 || sum == sum)
		//		myField.setText("");
				
				}
				catch (NumberFormatException nfe) { //catching anything thats not a number 
               		JOptionPane.showMessageDialog(null,"input must be a number.");
            	}myField.setText(null);	// clearing the myField after the showMessageDialog pops to input must be a number	
	
		}

} 
