# schedulerjava
import java.util.Calendar;
import java.util.Timer;
import java.util.TimerTask;

public class schedule {
    public static void main(String[] args) {
		Timer timer = new Timer();
		TimerTask tt = new TimerTask(){
			public void run(){
				Calendar cal = Calendar.getInstance(); 
 
			int hour = cal.get(Calendar.HOUR_OF_DAY); 
                        
				if(hour == 03)
					System.out.println(" Hi its 3 AM" );
				}

		};
		timer.schedule(tt, 1000, 1000*18); 
                timer.cancel();
	}
}
