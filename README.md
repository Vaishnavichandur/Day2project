# Day1project
Day 1 project code
<html>
    <title>21P61A0546</title>
    <style>
        label{
            font-size: 20;
           
        }
        body{
            text-align:center;
            background-color:azure;
        }
        input[type=email],input[type=text],input[type=tel],input[type=password]{
            border-style:solid;
            width: 300px; 
            height: 30px;
        }
        input[type=submit]{
            background-color:limegreen;
        }
        
    </style>
    <body>
        <img src="C:\Users\Vaishnavi\OneDrive\Pictures\Screenshots\Screenshot 2023-10-12 103341.png" style="width: 150px; height: 80px" float="right" >
        <h2 ><b> Find a job &grow your career</b></h2>>
        
         <form name="f1" method="post" action="#" onsubmit="return myfunc()">
            <fieldset>

        <label for="fname"> Full name </label> <br>
        <input type="text" id="fname" name="fname" placeholder="What is your name?" ><br><br>

    <label for="mail"> Email ID </label><br>
    <input type="email" name="mail" placeholder="Tell us your Email ID"  required> <p style="text-align:center;color:grey;"><small>We'll send you relevant jobs in your mail</small></p><br>
        <label for="pwd"> Password </label><br>
        <input type="password" id="pwd" name="pwd" placeholder="Create a password for your account" ><p style="text-align:center;color:grey;"><small>Minimum 6 characters required</small></p><br>

        <label for="mbnum">Mobile number</label><br>
        <input type="tel" id="mobnum" name="mobnun" placeholder="+91 Mobile Number" required ><p style="text-align:center;color:grey;"><small>Recruiters will call you on this number</small></p><br><br>
<label for="wrk">Work status</label><br>
<input type="radio" name="wrk1" >I'm experienced
<input type="radio" name="wrk2" >I'm a fresher<br><br>
<label for="resm">Resume </label><br>
<input type="file" name="file"><p style="text-align:center;color:grey;"><small>*Doc,DOCX,RTF | Max: 2MB <br> Recruiters give first preference to candidates who have a resume</small></p><br>
    <label for="terms"></label> <br>
    <input type="checkbox" name="r1"> Send me important Updates on Whatsapp <br><br>

            <small>By clicking Register, you agree to the Terms and Conditions & Privacy Policy of Naukri.com</small><br>

            <input type="submit" value="submit">
            </fieldset>
         </form>
    </body>
<script>
        function myfunc(){
            let p1=f1.pwd.value;
            if(f1.fname.value==null||f1.fname.value==""){
                alert("pls enter name");
                return false;

            }
            else if(p1.length<6){
                alert("password must be atleast 6 chars");
            return false; 
        }
        else if(f1.wrk1.checked){
            prompt("enter experience");
            return true;
        }
        else if(!f1.r1.checked){
            confirm("to get notified further click yes");
            return false;
        }

        }



        
    </script>
</html>
