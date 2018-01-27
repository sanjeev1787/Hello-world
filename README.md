/**
* create class for generating Bcrypt password to raw password
*/

import org.springframework.security.crypto.bcrypt.BCryptPasswordEncoder;

public class QuickPasswordEncodingGenerator {

	/**
	 * @param args
	 */

	public static void main(String[] args) {
		String password = "abc125";
		BCryptPasswordEncoder passwordEncoder = new BCryptPasswordEncoder();
		String enpass = passwordEncoder.encode(password);
		System.out.println(passwordEncoder.encode(password));
		
	}

}
