package phuongtrinhbac2;

import java.awt.BorderLayout;
import java.awt.EventQueue;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;
import java.awt.event.KeyAdapter;
import java.awt.event.KeyEvent;

import javax.swing.JFrame;
import javax.swing.JPanel;
import javax.swing.border.EmptyBorder;
import javax.swing.JLabel;
import javax.swing.JOptionPane;
import javax.swing.JTextField;
import javax.swing.JButton;
import java.awt.Color;

public class phuongtrinh extends JFrame {

	private JPanel txtGiai;
	private JTextField txtA;
	private JTextField txtB;
	private JTextField txtC;
	private JTextField txt_Giai;	

	/**
	 * Launch the application.
	 */
	public static void main(String[] args) {
		EventQueue.invokeLater(new Runnable() {
			public void run() {
				try {
					phuongtrinh frame = new phuongtrinh();
					frame.setVisible(true);
				} catch (Exception e) {
					e.printStackTrace();
				}
			}
		});
	}

	/**
	 * Create the frame.
	 */
	public phuongtrinh() {
		setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
		setBounds(100, 100, 450, 300);
		txtGiai = new JPanel();
		txtGiai.setBorder(new EmptyBorder(5, 5, 5, 5));
		setContentPane(txtGiai);
		txtGiai.setLayout(null);
		
		JLabel lbA = new JLabel("Nh\u1EADp a :");
		lbA.setBounds(47, 62, 60, 14);
		txtGiai.add(lbA);
		
		txtA = new JTextField();
		txtA.setBounds(129, 59, 137, 20);	
		txtGiai.add(txtA);
		txtA.setColumns(10);
		
		txtB = new JTextField();
		txtB.setColumns(10);
		txtB.setBounds(129, 101, 137, 20);
		txtGiai.add(txtB);
		
		txtC = new JTextField();
		txtC.setColumns(10);
		txtC.setBounds(130, 143, 137, 20);	
		txtGiai.add(txtC);
		
		JLabel lbB = new JLabel("Nh\u1EADp b :");
		lbB.setBounds(47, 104, 60, 14);
		txtGiai.add(lbB);
		
		JLabel lbC = new JLabel("Nh\u1EADp	 c : ");
		lbC.setBounds(47, 146, 74, 14);
		txtGiai.add(lbC);
		
		JButton btnGiai = new JButton("Giai");
		btnGiai.setForeground(Color.DARK_GRAY);
		btnGiai.setBounds(32, 193, 89, 23);
		txtGiai.add(btnGiai);
	
		btnGiai.addActionListener(new ActionListener() {
                 
			public void actionPerformed(ActionEvent e) {
         if(btnGiai.getText().equalsIgnoreCase("Giai")) {
        	 btnGiai.setText("Lam lai");
        	 int a = Integer.parseInt(txtA.getText());
				int b = Integer.parseInt(txtB.getText());
				int c = Integer.parseInt(txtC.getText());
				int d = (b*b - 4*a*c);
			
				if(d > 0)
				{
				int x1,x2;
				x1=(int) (((-b+Math.sqrt(d)))/2*a);
				x2=(int) (((-b-Math.sqrt(d)))/2*a);
					txt_Giai.setText("x1 =" +x1+",x2="+x2);
				
				}
				else if(d < 0) JOptionPane.showMessageDialog(btnGiai, "The equation don't have root");
        	 
        	 
        	 
        	 
         }
         else { btnGiai.setText("Giai");
         txtA.setText("");
			txtB.setText("");
			txtC.setText("");
            txt_Giai.setText("");
         }
				
				
					
				
			}
		});
		
		txt_Giai = new JTextField();
		txt_Giai.setBounds(136, 174, 130, 61);
		txtGiai.add(txt_Giai);
		txt_Giai.setColumns(10);
		
		JLabel lblGiiPhngTrnh = new JLabel("Gi\u1EA3i ph\u01B0\u01A1ng tr\u00ECnh b\u1EADc 2");
		lblGiiPhngTrnh.setBounds(157, 24, 151, 14);
		txtGiai.add(lblGiiPhngTrnh);
		
		txtC.addKeyListener(new KeyAdapter() {
			@Override
			public void keyPressed(KeyEvent e) {
				if(e.getKeyCode() == KeyEvent.VK_ENTER)
				{   btnGiai.setText("Lam lai");
					int a = Integer.parseInt(txtA.getText());
					int b = Integer.parseInt(txtB.getText());
					int c = Integer.parseInt(txtC.getText());
					int d = (b*b - 4*a*c);
				
					if(d > 0)
					{
						int x1,x2;
						x1=(int) (((-b+Math.sqrt(d)))/2*a);
						x2=(int) (((-b-Math.sqrt(d)))/2*a);
							txt_Giai.setText("x1 =" +x1+",x2="+x2);
					}
					else if(d < 0) JOptionPane.showMessageDialog(txtC, "The equation is no root");
				}
			}
		});
		
		
	}

}
	

