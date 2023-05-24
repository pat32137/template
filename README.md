# template

file_html = open("mail.html", "w")


b4buildtype="""<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<meta http-equiv="X-UA-Compatible" content="IE=edge" />
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>TAREB Email Template</title>
<style type="text/css">
	@import url('https://fonts.googleapis.com/css2?family=Roboto+Condensed:wght@700&display=swap'); 
	table, th, td {
        border: 3px solid white;
        border-collapse: collapse;
        border-radius: 10px;
      }
      th {
        background-color: #8adcdc;
      }
      td{
        background-color: #adcece;
      }
</style>

</head>
<body>
			
<!-- TOP SECTION -->
    <table width="80%">
        <tr>"""
        
color=        """<td style="background-color:#8adcdc;border-radius: 100px;">"""
b4inserttype=                """<h1 style="padding-left: 40px ;font-family: Arial">"""
b4link1=    """</h1>
            </td>
        </tr>
    </table>
    <br>
	<table width="80%" >
        <tr><h1 style="padding-left: 40px ;font-family: Arial">


        </h1></tr>
		<tr>
            <td width="30%">
                <h2 style="padding-left: 30px ; font-family:Arial;font-size: 15pt" >URL:</h2>
            </td>
            <td>
                <h2 style="padding-left: 10px ; font-family:Arial ; font-size: 13pt; font-weight: 300">"""


b4project_name1="""</h2>
            </td>
        </tr>
        <tr>
            <td width="30%">
                <h2 style="padding-left: 30px ; font-family:Arial; font-size: 15pt">PROJECT:</h2>
            </td>
            <td>
                <h2 style="padding-left: 10px ; font-family:Arial ; font-size: 13pt; font-weight: 300">"""
                

b4datetime1="""</h2>
            </td>
        </tr>
        <tr>
            <td width="40%">
                <h2 style="padding-left: 30px ; font-family:Arial; font-size: 15pt">DATE:</h2>
            </td>
            <td>
                <h2 style="padding-left: 10px ; font-family:Arial ; font-size: 13pt; font-weight: 300">"""

b4time_period1="""</h2>
            </td>
        </tr>
        <tr>
            <td width="30%">
                <h2 style="padding-left: 30px ; font-family:Arial ; font-size: 15pt">DURATION:</h2>
            </td>
            <td>
                <h2 style="padding-left: 10px ; font-family:Arial ; font-size: 13pt; font-weight: 300">"""
        
b4statement1="""</h2>
            </td>
        </tr>
        <tr>
            <td width="30%">
                <h2 style="padding-left: 30px ; font-family:Arial; font-size: 15pt ">CAUSE:</h2>
            </td>
            <td>
                <h2 style="padding-left: 10px ; font-family:Arial ; font-size: 13pt; font-weight: 300">"""

b4var1="""</h2>
            </td>
        </tr>
	</table>
    <br>
    <hr>
    <table width="80%">
        <h1 style="padding-left: 40px; font-family:Arial">Test Summary</h1>
        <tr>
            <th width="20%">
                <h2 style="padding-left: 10px ; font-family:Arial ; font-size: 15pt">Total</h2>
            </th>
            <th width="20%">
                <h2 style="padding-left: 10px ; font-family:Arial ; font-size: 15pt">Failed</h2>
            </th>
            <th width="20%">
                <h2 style="padding-left: 10px ; font-family:Arial ; font-size: 15pt">Passed</h2>
            </th>
            <th width="20%">
                <h2 style="padding-left: 10px ; font-family:Arial ; font-size: 15pt">Pass%</h2>
            </th>
        </tr>
        <tr>
            <td>
                <h2 width="20%" style="text-align :center; font-family:Arial ; font-size: 13pt; font-weight: 300;">"""
                
b4var2="""</h2>
            </td>
            <td>
                <h2 width="20%" style="text-align :center; font-family:Arial ; font-size: 13pt; font-weight: 300;">"""
        
b4var3="""</h2>
            </td>
            <td>
                <h2 width="20%" style="text-align :center; font-family:Arial ; font-size: 13pt; font-weight: 300;">"""
        
b4var4="""</h2>
            </td>
            <td>
                <h2 width="20%" style="text-align :center; font-family:Arial ; font-size: 13pt; font-weight: 300;">"""
            
b4test_type1="""</h2>
            </td>
        </tr>

    </table>
    <br>
    <hr>
    <table width="80%">
        <h1 style="padding-left: 40px; font-family: Arial">METADATA</h1>
        <tr>
            <td width="40%">
                <h2 style="padding-left: 30px ; font-family:Arial; font-size: 15pt" >test_type:</h2>
            </td>
            <td>
                <h2 style="padding-left: 10px ; font-family:Arial ; font-size: 13pt; font-weight: 300">"""

b4release_no1="""</h2>
            </td>
        </tr>
        <tr>
            <td width="40%">
                <h2 style="padding-left: 30px ; font-family:Arial; font-size: 15pt">release_no:</h2>
            </td>
            <td>
                <h2 style="padding-left: 10px ; font-family:Arial ; font-size: 13pt; font-weight: 300">"""

b4commit_appversion="""</h2>
            </td>
        </tr>
        <tr>
            <td width="40%">
                <h2 style="padding-left: 30px ; font-family:Arial ; font-size: 15pt">commit_appversion:</h2>
            </td>
            <td>
                <h2 style="padding-left: 10px ; font-family:Arial ; font-size: 13pt; font-weight: 300">"""
    
b4emte_minute_per_tc="""</h2>
            </td>
        </tr>
        <tr>
            <td width="40%">
                <h2 style="padding-left: 30px ; font-family:Arial; font-size: 15pt ">emte_minute_per_tc:</h2>
            </td>
            <td>
                <h2 style="padding-left: 10px ; font-family:Arial ; font-size: 13pt; font-weight: 300">"""
                
b4test_name="""</h2>
            </td>
        </tr>
    </table>
    <br>
    <hr>
    <table width="80%">
        <h1 style="padding-left: 40px; font-family: Arial;">Failed Test Execution Details</h1>
        <tr>
            <th width="60%">
                <h2 style=" font-family:Arial ; text-align :center; font-size: 15pt">Test name</h2>
            </th>
            <th width="20%">
                <h2 style=" font-family:Arial ; text-align :center; font-size: 15pt">Status</h2>
            </th>
            <th width="20%">
                <h2 style=" font-family:Arial ; text-align :center; font-size: 15pt">Duration</h2>
            </th>
        </tr>"""
startofloop="""<tr>
            <td>
                <h2 style="padding-left: 10px ; font-family:Arial ; font-size: 13pt; font-weight: 300">"""
                
b4test_status="""</h2>
            </td>
            <td>
                <h2 style="padding-left: 10px ; font-family:Arial ; font-size: 13pt ; font-weight: 300; text-align:center ">"""
    
b4duration="""</h2>
            </td>
            <td>
                <h2 style="padding-left: 10px ; font-family:Arial ; font-size: 13pt ; font-weight: 300; text-align:center ">"""

endloop="""</h2>
            </td>
        </tr>"""
endofcode="""</table>

</body>
</html>"""


buildtype=" BUILD STABLE "
link1="abc"
project_name1="dog"
datetime1="cat"
time_period1="days"
statement1="frog"
var1="a"
var2="b"
var3="c"
var4="d"
test_type="bcd"
release_no="duck"
commit_appversion="cow"
emte_minute_per_tc="weeks"
testname="case"
test_status="pass"
duration="month"




htmlcode=b4buildtype+color+buildtype+b4link1+link1+b4project_name1+project_name1+b4datetime1+datetime1+b4time_period1+time_period1+b4statement1+statement1+b4var1+var1+b4var2+var2+b4var3+var3+b4var4+var4+b4test_type1+test_type+b4release_no1+release_no+b4commit_appversion+commit_appversion+b4emte_minute_per_tc+emte_minute_per_tc+b4test_name+testname+b4test_status+test_status+b4duration+duration+endofcode



file_html.write(htmlcode)
