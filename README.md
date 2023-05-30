# java_practicals_02
All java practicals programs
import java.awt.*;
import java.awt.event.*;
public class MouseDemo extends Frame implements MouseListener {
	Label l;
	MouseDemo() {

		l = new Label();
		l.setBackground(Color.GREEN);
		l.setBounds(25, 60, 250, 30);
		l.setAlignment(Label.CENTER);
		this.add(l);
		this.setSize(300, 300);
		this.setLayout(null);
		this.setVisible(true);
		this.addMouseListener(this);

	}
	public static void main(String[] args) {
		new MouseDemo();
	}

	public void mouseClicked(MouseEvent e) {
		l.setText("Mouse Clicked");
	}

	public void mousePressed(MouseEvent e) {
		l.setText("Mouse Pressed");
	}

	public void mouseReleased(MouseEvent e) {
		l.setText("Mouse Released");
	}

	public void mouseEntered(MouseEvent e) {
		l.setText("Mouse Entered");

	}

	public void mouseExited(MouseEvent e) {
		l.setText("Mouse Exited");
	}
}


