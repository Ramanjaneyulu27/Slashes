# Slashes
/*Input: path = "/home//foo/"
Output: "/home/foo"
Explanation: In the canonical path, multiple consecutive slashes are replaced by a single one.*/ And if there is any slash at the end of the string remove it.

//////CODE STARTS FROM HERE//////

public class Pathf {

	public static void main(String[] args) {
		String s="/home//foo/";
		char ch[]=s.toCharArray();
			
			if(ch[ch.length-1]=='/' ) {
				for(int k=0;k<ch.length-1;k++) {
				
						
					if(ch[k]=='/' && ch[k+1]=='/' ) {
						continue;
						}
					else {
						System.out.print(ch[k]);
					}
				}	
			}
			
			else {
					for(int i=0;i<ch.length;i++) {
						if(ch[i]=='/' && ch[i+1]=='/' ) {
							continue;
							}
						else {
							System.out.print(ch[i]);
						}
					}
			}
	}

}
