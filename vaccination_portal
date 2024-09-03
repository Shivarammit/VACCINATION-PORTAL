import mysql.connector
import random
import math
con=mysql.connector.connect(host='localhost',user='root',database='cs_project',password='srnair1234',charset='utf8')
if con.is_connected()==False:
    print("Error in connection")
else:
    print("Connection successful")
cursor=con.cursor()
print("*******************VACCINATION PORTAL***************************")
register=print("1.REGISTER")
sign_in=print("2.SIGN IN")
hospital_sign_in=print("3.HOSPITAL SIGN IN")
check_availibility_of_vaccine=print("4.CHECK AVAILABILITY OF VACCINE")
about_vaccine=print("5.ABOUT VACCINES")
contact_us=print("6.CONTACT US")
page1=input("ENTER YOUR INPUT(1/2/3/4/5/6):")
if page1 in ('1'):
    print("********REGISTER YOURSELF*****************")
    print("NOTE:TYPE EVERYTHING IN CAPS")
    name=input("NAME:")
    age=int(input("AGE:"))
    aadhar_no=int(input("AADHAR NO:"))
    mobile_no=int(input("MOBILE NO:"))
    st1="insert into patient_details values('{}',{},{},{})".format(name,age,aadhar_no,mobile_no)
    cursor.execute(st1)
    con.commit()
    print("REGISTERED SUCCESSFULLY")
    print("Do you want to sign in?")
    print('1.yes')
    print('2.no')
    page2=input("Enter your input(1/2):")
    if page2 in ('1'):
        print("************SIGN IN HERE***************")
        name = input("ENTER YOUR NAME:")
        password = int(input("MOBILE NO:"))
        st2 = "select name,age from patient_details where mobile_no={}".format(password)
        cursor.execute(st2)
        data = cursor.fetchall()
        count = cursor.rowcount
        for row in data:
            print(row)
        print("1.DOSE 1")
        print("2.DOSE 2")
        dose = input("ENTER YOUR INPUT(1/2):")
        if dose in ('1'):
            state = print("CHOOSE YOUR STATE")
            print("1.TAMILNADU")
            print("2.KERALA")
            print("3.ANDHRA PRADESH")
            print("4.KARNATAKA")
            state = input("ENTER YOUR STATE:")
            if state in ('TAMILNADU'):
                print("ENTER YOUR CITY:")
                print("1.KARUR")
                print('2.CHENNAI')
                print('3.TRICHY')
                print('4.COIMBATORE')
                print("5.MADURAI")
                city = input("ENTER YOUR CITY):")
                if city in ('KARUR'):
                    print("CHOOSE YOUR HOSPITAL:")
                    print("1.APOLLO HOSPITAL")
                    print("2.KARUR GH")
                    print("3.GANDHI GRAMAM GH")
                    hospital_name = input("ENTER YOUR HOSPITAL:")
                    if hospital_name in ('APOLLO HOSPITAL'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('KARUR GH'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('GANDHI GRAMAM GH'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                if city in ('CHENNAI'):
                    print("CHOOSE YOUR HOSPITAL:")
                    print("1.APOLLO HOSPITAL")
                    print("2.FORTIS GROUP OF HOSPITALS")
                    print("3.RAJIV GANDHI GOVERNMENT GENERAL HOSPITAL")
                    hospital_name = input("ENTER YOUR HOSPITAL:")
                    if hospital_name in ('APOLLO HOSPITAL'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('FORTIS GROUP OF HOSPITALS'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('RAJIV GANDHI GOVERNMENT GENERAL HOSPITAL'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                if city in ('TRICHY'):
                    print("CHOOSE YOUR HOSPITAL:")
                    print("1.JEYAM MULTI SPECIALLITY HOSPITAL")
                    print("2.ABC HOSPITAL")
                    print("3.TRICHY GH")
                    hospital_name = input("ENTER YOUR HOSPITAL:")
                    if hospital_name in ('JEYAM MULTI SPECIALITY HOSPITAL'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('ABC HOSPITAL'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('TRICHY GH'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                if city in ('COIMBATORE'):
                    print("CHOOSE YOUR HOSPITAL:")
                    print("1.KMCH")
                    print("2.KG HOSPITAL")
                    print("3.COIMBATORE GH")
                    hospital_name = input("ENTER YOUR HOSPITAL:")
                    if hospital_name in ('KMCH'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('KG HOSPITAL'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('COIMBATORE GH'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                if city in ('MADURAI'):
                    print("CHOOSE YOUR HOSPITAL:")
                    print("1.LAKSHANA MULTI SPECIALITY HOSPITAL")
                    print("2.VELLAMAL GROUP OF HOSPITALS")
                    print("3.MADURAI GH")
                    hospital_name = input("ENTER YOUR HOSPITAL:")
                    if hospital_name in ('LAKSHANA MULTI SPECIALITY HOSPITAL'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('VELLAMAL GROUP OF HOSPITALS'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('MADURAI GH'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
            if state in ('KERALA'):
                print("ENTER YOUR CITY")
                print("1.PALAKAD")
                print('2.COCHIN')
                print('3.THIRUVANANTHAPURAM')
                print('4.THRISSUR')
                print("5.SHORNUR")
                city = input("Enter your CITY:")
                if city in ('PALAKAD'):
                    print("CHOOSE YOUR HOSPITAL:")
                    print("1.THANGAM HOSPITALS")
                    print("2.TRINITY")
                    print("3.PALAKAD GH")
                    hospital_name = input("ENTER YOUR HOSPITAL:")
                    if hospital_name in ('THANGAM HOSPITALS'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('TRINITY'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('PALAKAD GH'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                if city in ('THIRUVANANTHAPURAM'):
                    print("CHOOSE YOUR HOSPITAL:")
                    print("1.KIIMS HOSPITAL")
                    print("2.SIMANS HOSPIAL")
                    print("3.TRIVANDRUM GH")
                    hospital_name = input("ENTER YOUR HOSPITAL:")
                    if hospital_name in ('KIIMS HOSPITAL'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('SIMANS HOSPITAL'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('TRIVANDRUM GH'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                if city in ('COCHIN'):
                    print("CHOOSE YOUR HOSPITAL:")
                    print("1.VPS LAKSHORE HOSPITALS")
                    print("2.ASTER MEDICITY")
                    print("3.COCHIN GH")
                    hospital_name = input("ENTER YOUR HOSPITAL:")
                    if hospital_name in ('VPS LAKSHORE HOSPITALS'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('ASTER MEDICITY'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('COCHIN GH'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                if city in ('THRISSUR'):
                    print("CHOOSE YOUR HOSPITAL:")
                    print("1.ELITE MISSION HOSPITAL")
                    print("2.DAYA GENERAL HOSPITAL")
                    print("3.THRISSUR GH")
                    hospital_name = input("ENTER YOUR HOSPITAL:")
                    if hospital_name in ('ELITE MISSION HOSPITAL'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('DAYA GENERAL HOSPITAL'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('THRISSUR GH'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                if city in ('SHORNUR'):
                    print("CHOOSE YOUR HOSPITAL:")
                    print("1.NHIMS HOSPITALS")
                    print("2.ALISTER MEDICAL CENTER")
                    print("3.SHORNUR GH")
                    hospital_name = input("ENTER YOUR HOSPITAL:")
                    if hospital_name in ('NHIMS HOSPITALS'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('ALISTER MEDICAL CENTER'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('SHORNUR GH'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
            if state in ('ANDHRA PRADESH'):
                print("ENTER YOUR CITY")
                print("1.VIZAG")
                print('2.TIRUPATI')
                print('3.CHITTOOR')
                print('4.KURNOOL')
                print("4.SRIKAKULAM")
                city = input("ENTER YOUR CITY:")
                if city in ('VIZAG'):
                    print("CHOOSE YOUR HOSPITAL:")
                    print("1.APOLLO HOSPITAL")
                    print("2.VIZAG GH")
                    hospital_name = input("ENTER YOUR HOSPITAL:")
                    if hospital_name in ('APOLLO HOSPITAL'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('VIZAG GH'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                if city in ('TIRUPATI'):
                    print("CHOOSE YOUR HOSPITAL:")
                    print("1.NARAYANDRI HOSPITALS")
                    print("2.AMARAVATHI HOSPITAL")
                    print("3.TIRUPATI GOVERNMENT GENERAL HOSPITAL")
                    hospital_name = input("ENTER YOUR HOSPITAL:")
                    if hospital_name in ('NARAYANDRI HOSPITALS'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('AMARAVATHI HOSPITAL'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('TIRUPATI GOVERNMENT GENERAL HOSPITAL'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                if city in ('CHITTOOR'):
                    print("CHOOSE YOUR HOSPITAL:")
                    print("1.GLOBAL MULTI SPECIALITY HOSPITAL")
                    print("2.ESI HOSPITAL")
                    print("3.CHITTOOR GH")
                    hospital_name = input("ENTER YOUR HOSPITAL:")
                    if hospital_name in ('GLOBAL MULTI SPECIALITY HOSPITAL'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('ESI HOSPITAL'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('CHITTOOR GH'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                if city in ('KURNOOL'):
                    print("CHOOSE YOUR HOSPITAL:")
                    print("1.MEDICARE HOSPITAL")
                    print("2.OMNI HOSPITALS")
                    print("3.KURNOOL GH")
                    hospital_name = input("ENTER YOUR HOSPITAL:")
                    if hospital_name in ('MEDICARE HOSPITAL'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('OMNI HOSPITALS'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('KURNOOL GH'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                if city in ('SRIKULAM'):
                    print("CHOOSE YOUR HOSPITAL:")
                    print("1.MEDICOVER HOSPITAL")
                    print("2.KIIMS HOSPITAL")
                    print("3.SRIKULAM GH")
                    hospital_name = input("ENTER YOUR HOSPITAL:")
                    if hospital_name in ('MEDICOVER HOSPITAL'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('KIIMS HOSPITAL'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('SRIKULAM GH'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
            if state in ('4'):
                print("ENTER YOUR CITY:")
                print("1.BANGALORE")
                print('2.MYSORE')
                print('3.MANGALORE')
                print('4.DHARWAD')
                print("5.BELAGAVI")
                city = input("ENTER YOUR CITY:")
                if city in ('BANGALORE'):
                    print("CHOOSE YOUR HOSPITAL:")
                    print("1.MANIPAL HOSPITAL")
                    print("2.BENGALURU GH")
                    hospital_name = input("ENTER YOUR HOSPITAL:")
                    if hospital_name in ('MANIPAL HOSPITAL'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('BANGALORE GH'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                if city in ('MYSORE'):
                    print("CHOOSE YOUR HOSPITAL:")
                    print("1.COLOUMBIA ASIA HOSPITAL")
                    print("2.APOLLO HOSPITAL")
                    print("3.MYSORE GOVERNMENT GENERAL HOSPITAL")
                    hospital_name = input("ENTER YOUR HOSPITAL:")
                    if hospital_name in ('COLOUMBIA ASIA HOSPITAL'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('APOLLO HOSPITAL'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('MYSORE GOVERNMENT GENERAL HOSPITAL'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                if city in ('MANGALORE'):
                    print("CHOOSE YOUR HOSPITAL:")
                    print("1.HIGHLAND HOSPITAL")
                    print("2.KMC HOSPITAL")
                    print("3.MANGALORE GH")
                    hospital_name = input("ENTER YOUR HOSPITAL:")
                    if hospital_name in ('HIGHLAND HOSPITAL'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('KMC HOSPITAL'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('MANGALORE GH'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                if city in ('DHARWAD'):
                    print("CHOOSE YOUR HOSPITAL:")
                    print("1.SPANDANA HOSPITALS")
                    print("2.SHREYA HOSPITALS")
                    print("3.DHARWAD GH")
                    hospital_name = input("ENTER YOUR HOSPITAL:")
                    if hospital_name in ('SPANDANA HOSPITALS'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('SHREYA HOSPITALS'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('DHARWAD GH'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                if city in ('BELAGAVI'):
                    print("CHOOSE YOUR HOSPITAL:")
                    print("1.SUPER SPECIALITY HOSPITALS")
                    print("2.YASH HOSPITAL")
                    print("3.BELAGAVI GH")
                    hospital_name = input("ENTER YOUR HOSPITAL:")
                    if hospital_name in ('SUPER SPECIALITY HOSPITAL'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('YASH HOSPITAL'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
                    if hospital_name in ('BELAGAVI GH'):
                        print("CHOOSE YOUR VACCINE:")
                        print("1.COVISHIELD")
                        print("2.COVAXIN")
                        print("3.SPUTNIK V")
                        vaccine_name = input("ENTER YOUR VACCINE:")
            date = input("ENTER YOUR DATE OF VACCINATION(YYYY-MM-DD):")
            st4 = "insert into dose_details(name,mobile_no,dose1_vaccinated_date,state,city,vaccine_name,hospital_name)values('{}',{},'{}','{}','{}','{}','{}')".format(
                name, password, date, state, city, vaccine_name, hospital_name)
            print("******CONFIRMATION*******")
            print("DO YOU WANT TO CONTINUE?")
            print("1.YES")
            print("2.NO")
            page81 = input("ENTER YOUR INPUT HERE(1/2):")
            if page81 in ('1'):
                cursor.execute(st4)
                con.commit()
                print("YOU HAVE REGISTERED YOUR SLOT FOR VACCINATION ON", date, "at", hospital_name, ",", city)
        if dose in ('2'):
            date1 = input("ENTER YOUR DATE TO BE VACCINATED(YYYY-MM-DD):")
            st5 = "update dose_details set dose2_vaccinated_date='{}' where mobile_no={}".format(date1, password)
            cursor.execute(st5)
            con.commit()
if page1 in ('2'):
   print("************SIGN IN HERE***************")
   name=input("ENTER YOUR NAME:")
   password=int(input("MOBILE NO:"))
   st2="select name,age from patient_details where mobile_no={}".format(password)
   cursor.execute(st2)
   data = cursor.fetchall()
   count = cursor.rowcount
   for row in data:
       print(row)
   print("1.DOSE 1")
   print("2.DOSE 2")
   dose=input("ENTER YOUR INPUT(1/2):")
   if dose in ('1'):
      state = print("CHOOSE YOUR STATE")
      print("1.TAMILNADU")
      print("2.KERALA")
      print("3.ANDHRA PRADESH")
      print("4.KARNATAKA")
      state=input("ENTER YOUR INPUT:")
      if state in ('TAMILNADU'):
        print("ENTER YOUR CITY:")
        print("1.KARUR")
        print('2.CHENNAI')
        print('3.TRICHY')
        print('4.COIMBATORE')
        print("5.MADURAI")
        city=input("ENTER YOUR INPUT):")
        if city in ('KARUR'):
           print("CHOOSE YOUR HOSPITAL:")
           print("1.APOLLO HOSPITAL")
           print("2.KARUR GH")
           print("3.GANDHI GRAMAM GH")
           hospital_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('APOLLO HOSPITAL'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('KARUR GH'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('GANDHI GRAMAM GH'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               vaccine_name = input("ENTER YOUR INPUT:")
        if city in ('CHENNAI'):
           print("CHOOSE YOUR HOSPITAL:")
           print("1.APOLLO HOSPITAL")
           print("2.FORTIS GROUP OF HOSPITALS")
           print("3.RAJIV GANDHI GOVERNMENT GENERAL HOSPITAL")
           hospital_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('APOLLO HOSPITAL'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('FORTIS GROUP OF HOSPITALS'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('RAJIV GANDHI GOVERNMENT GENERAL HOSPITAL'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name=input("ENTER YOUR INPUT:")
        if city in ('TRICHY'):
           print("CHOOSE YOUR HOSPITAL:")
           print("1.JEYAM MULTI SPECIALLITY HOSPITAL")
           print("2.ABC HOSPITAL")
           print("3.TRICHY GH")
           hospital_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('JEYAM MULTI SPECIALITY HOSPITAL'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('ABC HOSPITAL'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('TRICHY GH'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name=input("ENTER YOUR INPUT:")
        if city in ('COIMBATORE'):
           print("CHOOSE YOUR HOSPITAL:")
           print("1.KMCH")
           print("2.KG HOSPITAL")
           print("3.COIMBATORE GH")
           hospital_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('KMCH'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('KG HOSPITAL'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('COIMBATORE GH'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name=input("ENTER YOUR INPUT:")
        if city in ('MADURAI'):
           print("CHOOSE YOUR HOSPITAL:")
           print("1.LAKSHANA MULTI SPECIALITY HOSPITAL")
           print("2.VELLAMAL GROUP OF HOSPITALS")
           print("3.MADURAI GH")
           hospital_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('LAKSHANA MULTI SPECIALITY HOSPITAL'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('VELLAMAL GROUP OF HOSPITALS'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('MADURAI GH'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name=input("ENTER YOUR INPUT:")
      if state in ('KERALA'):
        print("ENTER YOUR CITY")
        print("1.PALAKAD")
        print('2.COCHIN')
        print('3.THIRUVANANTHAPURAM')
        print('4.THRISSUR')
        print("5.SHORNUR")
        city = input("Enter your input:")
        if city in ('PALAKAD'):
           print("CHOOSE YOUR HOSPITAL:")
           print("1.THANGAM HOSPITALS")
           print("2.TRINITY")
           print("3.PALAKAD GH")
           hospital_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('THANGAM HOSPITALS'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('TRINITY'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('PALAKAD GH'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name=input("ENTER YOUR INPUT:")
        if city in ('THIRUVANANTHAPURAM'):
           print("CHOOSE YOUR HOSPITAL:")
           print("1.KIIMS HOSPITAL")
           print("2.SIMANS HOSPIAL")
           print("3.TRIVANDRUM GH")
           hospital_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('KIIMS HOSPITAL'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('SIMANS HOSPITAL'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('TRIVANDRUM GH'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name=input("ENTER YOUR INPUT:")
        if city in ('COCHIN'):
           print("CHOOSE YOUR HOSPITAL:")
           print("1.VPS LAKSHORE HOSPITALS")
           print("2.ASTER MEDICITY")
           print("3.COCHIN GH")
           hospital_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('VPS LAKSHORE HOSPITALS'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('ASTER MEDICITY'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('COCHIN GH'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name=input("ENTER YOUR INPUT:")
        if city in ('THRISSUR'):
           print("CHOOSE YOUR HOSPITAL:")
           print("1.ELITE MISSION HOSPITAL")
           print("2.DAYA GENERAL HOSPITAL")
           print("3.THRISSUR GH")
           hospital_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('ELITE MISSION HOSPITAL'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('DAYA GENERAL HOSPITAL'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('THRISSUR GH'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name=input("ENTER YOUR INPUT:")
        if city in ('SHORNUR'):
           print("CHOOSE YOUR HOSPITAL:")
           print("1.NHIMS HOSPITALS")
           print("2.ALISTER MEDICAL CENTER")
           print("3.SHORNUR GH")
           hospital_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('NHIMS HOSPITALS'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('ALISTER MEDICAL CENTER'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('SHORNUR GH'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name=input("ENTER YOUR INPUT:")
      if state in ('ANDHRA PRADESH'):
        print("ENTER YOUR CITY")
        print("1.VIZAG")
        print('2.TIRUPATI')
        print('3.CHITTOOR')
        print('4.KURNOOL')
        print("4.SRIKAKULAM")
        city = input("Enter your input(1/2/3/4/5):")
        if city in ('VIZAG'):
           print("CHOOSE YOUR HOSPITAL:")
           print("1.APOLLO HOSPITAL")
           print("2.VIZAG GH")
           hospital_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('APOLLO HOSPITAL'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('VIZAG GH'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
        if city in ('TIRUPATI'):
           print("CHOOSE YOUR HOSPITAL:")
           print("1.NARAYANDRI HOSPITALS")
           print("2.AMARAVATHI HOSPITAL")
           print("3.TIRUPATI GOVERNMENT GENERAL HOSPITAL")
           hospital_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('NARAYANDRI HOSPITALS'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('AMARAVATHI HOSPITAL'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('TIRUPATI GOVERNMENT GENERAL HOSPITAL'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name=input("ENTER YOUR INPUT:")
        if city in ('CHITTOOR'):
           print("CHOOSE YOUR HOSPITAL:")
           print("1.GLOBAL MULTI SPECIALITY HOSPITAL")
           print("2.ESI HOSPITAL")
           print("3.CHITTOOR GH")
           hospital_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('GLOBAL MULTI SPECIALITY HOSPITAL'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('ESI HOSPITAL'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('CHITTOOR GH'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name=input("ENTER YOUR INPUT:")
        if city in ('KURNOOL'):
           print("CHOOSE YOUR HOSPITAL:")
           print("1.MEDICARE HOSPITAL")
           print("2.OMNI HOSPITALS")
           print("3.KURNOOL GH")
           hospital_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('MEDICARE HOSPITAL'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('OMNI HOSPITALS'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('KURNOOL GH'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name=input("ENTER YOUR INPUT:")
        if city in ('SRIKULAM'):
           print("CHOOSE YOUR HOSPITAL:")
           print("1.MEDICOVER HOSPITAL")
           print("2.KIIMS HOSPITAL")
           print("3.SRIKULAM GH")
           hospital_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('MEDICOVER HOSPITAL'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('KIIMS HOSPITAL'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('SRIKULAM GH'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name=input("ENTER YOUR INPUT:")
      if state in ('4'):
        print("ENTER YOUR CITY:")
        print("1.BANGALORE")
        print('2.MYSORE')
        print('3.MANGALORE')
        print('4.DHARWAD')
        print("5.BELAGAVI")
        city = input("Enter your input(1/2/3/4/5):")
        if city in ('BANGALORE'):
           print("CHOOSE YOUR HOSPITAL:")
           print("1.MANIPAL HOSPITAL")
           print("2.BENGALURU GH")
           hospital_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('MANIPAL HOSPITAL'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('BANGALORE GH'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
        if city in ('MYSORE'):
           print("CHOOSE YOUR HOSPITAL:")
           print("1.COLOUMBIA ASIA HOSPITAL")
           print("2.APOLLO HOSPITAL")
           print("3.MYSORE GOVERNMENT GENERAL HOSPITAL")
           hospital_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('COLOUMBIA ASIA HOSPITAL'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('APOLLO HOSPITAL'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('MYSORE GOVERNMENT GENERAL HOSPITAL'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name=input("ENTER YOUR INPUT:")
        if city in ('MANGALORE'):
           print("CHOOSE YOUR HOSPITAL:")
           print("1.HIGHLAND HOSPITAL")
           print("2.KMC HOSPITAL")
           print("3.MANGALORE GH")
           hospital_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('HIGHLAND HOSPITAL'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('KMC HOSPITAL'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('MANGALORE GH'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name=input("ENTER YOUR INPUT:")
        if city in ('DHARWAD'):
           print("CHOOSE YOUR HOSPITAL:")
           print("1.SPANDANA HOSPITALS")
           print("2.SHREYA HOSPITALS")
           print("3.DHARWAD GH")
           hospital_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('SPANDANA HOSPITALS'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('SHREYA HOSPITALS'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('DHARWAD GH'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name=input("ENTER YOUR INPUT:")
        if city in ('BELAGAVI'):
           print("CHOOSE YOUR HOSPITAL:")
           print("1.SUPER SPECIALITY HOSPITALS")
           print("2.YASH HOSPITAL")
           print("3.BELAGAVI GH")
           hospital_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('SUPER SPECIALITY HOSPITAL'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('YASH HOSPITAL'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name = input("ENTER YOUR INPUT:")
           if hospital_name in ('BELAGAVI GH'):
               print("CHOOSE YOUR VACCINE:")
               print("1.COVISHIELD")
               print("2.COVAXIN")
               print("3.SPUTNIK V")
               vaccine_name=input("ENTER YOUR INPUT:")
      date = input("ENTER YOUR DATE OF VACCINATION(YYYY-MM-DD):")
      st4 = "insert into dose_details(name,mobile_no,dose1_vaccinated_date,state,city,vaccine_name,hospital_name)values('{}',{},'{}','{}','{}','{}','{}')".format(name,password,date,state,city,vaccine_name,hospital_name)
      print("CONFIRMATION")
      print("DO YOU WANT TO CONTINUE?")
      print("1.YES")
      print("2.NO")
      page81=input("ENTER YOUR INPUT HERE(1/2):")
      if page81 in ('1'):
        cursor.execute(st4)
        con.commit()
        print('loading....')
        print("YOU HAVE REGISTERED YOUR SLOT FOR DOSE 1 VACCINATION ON",date,"at",hospital_name,",",city)
   if dose in ('2'):
        date1=input("ENTER YOUR DATE TO BE VACCINATED(YYYY-MM-DD):")
        st5="update dose_details set dose2_vaccinated_date='{}' where mobile_no={}".format(date1,password)
        cursor.execute(st5)
        con.commit()
        print('loading....')
        print('YOU HAVE BOOKED YOUR SLOT OF DOSE 2 VACCINATION ON',date,'AT SAME HOSPITAL WHERE YOU HAVE VACCINATED DOSE 1')
elif page1 in ('3'):
    hospital_name=input("HOSPITAL NAME:")
    password1=input("PASSWORD:")
    st3="select hospital_name from hospital where hospital_name='{}'".format(hospital_name)
    cursor.execute(st3)
    data = cursor.fetchall()
    count = cursor.rowcount
    for row in data:
        print("             ***************WELCOME******************")
        print("HOSPITAL NAME:",hospital_name)
        print("1.DOSE 1 LIST")
        print("2.DOSE 2 LIST")
        page82=input("ENTER YOUR INPUT(1/2):")
        if page82 in ('1'):
            phone_no=int(input("MOBILE NO:"))
            print("1.MARK AS VACCINATED DOSE 1")
            print("2.REMOVE THIS PERSON FROM LIST")
            page83=input("ENTER YOUR INPUT(1/2):")
            if page83 in ('1'):
                print('loading....')
                print('MARKED SUCCESSFULLY')
                st5="update dose_details set dose1='{}' where mobile_no={}".format("VACCINATED",phone_no)
                cursor.execute(st5)
                con.commit()
            if page83 in ('2'):
                print("DO YOU WANT TO REMOVE THIS PERSON")
                print("1.YES")
                print("2.NO")
                page84=input("ENTER YOUR INPUT(1/2):")
                if page84 in ('1'):
                    st6="delete from dose_details where mobile_no={}".format(phone_no)
                    cursor.execute(st6)
                    con.commit()
                    print("THE PERSON INFORMATION HAS BEEN SUCCESSFULLY REMOVED FROM THE DATABASE")
        if page82 in ('2'):
            phone_no = int(input("MOBILE NO:"))
            print("1.MARK AS VACCINATED DOSE 2")
            print("2.REMOVE THIS PERSON FROM LIST")
            page83 = input("ENTER YOUR INPUT(1/2):")
            if page83 in ('1'):
                print('loading....')
                print('MARKED SUCCESSFULLY')
                st5 = "update dose_details set dose2='{}' where mobile_no={}".format("VACCINATED", phone_no)
                cursor.execute(st5)
                con.commit()
            if page83 in ('2'):
                print("DO YOU WANT TO REMOVE THIS PERSON")
                print("1.YES")
                print("2.NO")
                page84 = input("ENTER YOUR INPUT(1/2):")
                if page84 in ('1'):
                    st6 = "delete from dose_details where mobile_no={}".format(phone_no)
                    cursor.execute(st6)
                    con.commit()
                    print("THE PERSON INFORMATION HAS BEEN SUCCESSFULLY REMOVED FROM THE DATABASE")
elif page1 in ('4'):
    print("CHOOSE YOUR STATE")
    print("1.TAMILNADU")
    print("2.KERALA")
    print("3.ANDHRA PRADESH")
    print("4.KARNATAKA")
    page3=input("enter your input(1/2/3/4):")
    if page3 in ('1'):
        print("CHOOSE YOUR DISTRICT:")
        print("1.KARUR")
        print('2.CHENNAI')
        print('3.TRICHY')
        print('4.COIMBATORE')
        print("5.MADURAI")
        page4=input("ENTER YOUR INPUT(1/2/3/4/5):")
        if page4 in ('1'):
            print("CHOOSE YOUR HOSPITAL:")
            print("1.APOLLO HOSPITAL")
            print("2.KARUR GH")
            print("3.GANDHI GRAMAM GH")
            page5=input("ENTER YOUR INPUT(1/2/3):")
            if page5 in ('1'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                page6=input("ENTER YOUR INPUT(1/2):")
                if page6 in ('1'):
                    print("The number for slots available for covishield is",random.randint(0,50),"for today")
                    print("The cost of the vaccine is Rs.780")
                if page6 in('2'):
                    print("The number for slots available for covaxin is",random.randint(0,50),"for today")
                    print("The cost of the vaccine is Rs.780")
                if page5 in('2'):
                    print("CHOOSE YOUR VACCINE:")
                    print("1.COVISHIELD")
                    print("2.COVAXIN")
                    page7=input("ENTER YOUR INPUT(1/2)")
                    if page7 in ('1'):
                        print("The number of slots available for covishield is",random.randint(0,40),"for today")
                        print("The cost of the vaccine is free")
                    if page7 in ('2'):
                        print("The number of slots available for covaxin is",random.randint(0,40),"for today")
                        print("The cost of the vaccine is free")
                if page5 in ('3'):
                    print("CHOOSE YOUR VACCINE:")
                    print("1.COVISHIELD")
                    print("2.COVAXIN")
                    page8 = input("ENTER YOUR INPUT(1/2)")
                    if page8 in ('1'):
                        print("The number of slots available for covishield is", random.randint(0, 40), "for today")
                        print("The cost of the vaccine is free")
                    if page8 in ('2'):
                        print("The number of slots available for covaxin is", random.randint(0, 40), "for today")
                        print("The cost of the vaccine is free")
            else:
                    print("Error input")
        if page4 in ('2'):
            print("1.APOLLO HOSPITAL")
            print("2.FORTIS GROUP OF HOSPITALS")
            print("3.RAJIV GANDHI GOVERNMENT GENRAL HOSPITAL")
            page9=input("Enter your input(1/2/3):")
            if page9 in ('1'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page10=input("ENTER YOUR INPUT(1/2/3):")
                if page10 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.2400")
                if page10 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0,100), "for today")
                    print("The cost of the vaccine is Rs.2000")
                if page10 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0,100), "for today")
                    print("The cost of the vaccine is Rs.2200")
            if page9 in ('2'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page11 = input("ENTER YOUR INPUT(1/2/3):")
                if page11 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.2400")
                if page11 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.2000")
                if page11 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.2200")
            if page9 in ('3'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page12 = input("ENTER YOUR INPUT(1/2/3):")
                if page12 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
                if page12 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
                if page12 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0,100), "for today")
                    print("The cost of the vaccine is free")
        if page4 in ('3'):
            print("1.JEYAM MULTI SPECALITY HOSPITAL")
            print("2.ABC HOSPITAL")
            print("3.TRICHY GH")
            page13=input("ENTER YOUR INPUT(1/2/3):")
            if page13 in ('1'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page12 = input("ENTER YOUR INPUT(1/2/3):")
                if page12 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0,60), "for today")
                    print("The cost of the vaccine is 1600")
                if page12 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0,60), "for today")
                    print("The cost of the vaccine is 1600")
                if page12 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0,60), "for today")
                    print("The cost of the vaccine is 1600")
            if page13 in ("2"):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page12 = input("ENTER YOUR INPUT(1/2/3):")
                if page12 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0,60), "for today")
                    print("The cost of the vaccine is Rs.1600")
                if page12 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0,60), "for today")
                    print("The cost of the vaccine is Rs.1600")
                if page12 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0,60), "for today")
                    print("The cost of the vaccine is Rs.1600")
            if page13 in ("3"):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page12 = input("ENTER YOUR INPUT(1/2/3):")
                if page12 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1600")
                if page12 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1600")
                if page12 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                    print("The cost of the vaccine is Rs.1600")
        if page4 in ('4'):
            print("CHOOSE YOUR HOSPITAL:")
            print("1.KMCH")
            print("2.KG HOSPITAL")
            print("3.COIMBATORE GH")
            page14=input("ENTER YOUR INPUT(1/2/3):")
            if page14 in ('1'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page15 = input("ENTER YOUR INPUT(1/2/3):")
                if page15 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1800")
                if page15 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1600")
                if page15 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                    print("The cost of the vaccine is Rs.1600")
            if page14 in ('2'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page15 = input("ENTER YOUR INPUT(1/2/3):")
                if page15 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1800")
                if page15 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1800")
                if page15 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                    print("The cost of the vaccine is Rs.1800")
            if page14 in ('3'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page15 = input("ENTER YOUR INPUT(1/2/3):")
                if page15 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
                if page15 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
                if page15 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                    print("The cost of the vaccine is free")
        else:
            print("Error input")
        if page4 in ('5'):
            print("1.LAKSHANA MULTI SPECIALITITY HOSPITAL")
            print("2.VELLAMAL GROUP OF HOSPITALS")
            print("3.MADURAI GH")
            page17=input("ENTER YOUR INPUT(1/2/3):")
            if page17 in ('1'):
                    print("CHOOSE YOUR VACCINE:")
                    print("1.COVISHIELD")
                    print("2.COVAXIN")
                    print("3.SPUTNIK")
                    page15 = input("ENTER YOUR INPUT(1/2/3):")
                    if page15 in ('1'):
                        print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                        print("The cost of the vaccine is Rs.1800")
                    if page15 in ('2'):
                        print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                        print("The cost of the vaccine is Rs.1600")
                    if page15 in ('3'):
                        print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                        print("The cost of the vaccine is Rs.1600")
            if page17 in ('2'):
                    print("CHOOSE YOUR VACCINE:")
                    print("1.COVISHIELD")
                    print("2.COVAXIN")
                    print("3.SPUTNIK")
                    page15 = input("ENTER YOUR INPUT(1/2/3):")
                    if page15 in ('1'):
                        print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                        print("The cost of the vaccine is free")
                    if page15 in ('2'):
                        print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                        print("The cost of the vaccine is free")
                    if page15 in ('3'):
                        print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                        print("The cost of the vaccine is free")
            if page17 in ('3'):
                    print("CHOOSE YOUR VACCINE:")
                    print("1.COVISHIELD")
                    print("2.COVAXIN")
                    print("3.SPUTNIK")
                    page15 = input("ENTER YOUR INPUT(1/2/3):")
                    if page15 in ('1'):
                        print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                        print("The cost of the vaccine is free")
                    if page15 in ('2'):
                        print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                        print("The cost of the vaccine is free")
                    if page15 in ('3'):
                        print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                        print("The cost of the vaccine is free")
                    print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                    print("The cost of the vaccine is free")
    if page3 in ('2'):
        print("CHOOSE YOUR DISTRICT:")
        print("1.PALAKAD")
        print('2.COCHIN')
        print('3.THIRUVANANTHAPURAM')
        print('4.THRISSUR')
        print("5.SHORNUR")
        page18 = input("ENTER YOUR INPUT(1/2/3/4/5):")
        if page18 in ('1'):
            print("CHOOSE YOUR HOSPITAL:")
            print("1.THANGAM HOSPITALS")
            print("2.TRINITY")
            print("3.PALAKAD GH")
            page19 = input("ENTER YOUR INPUT(1/2/3):")
            if page19 in ('1'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                page20 = input("ENTER YOUR INPUT(1/2):")
                if page20 in ('1'):
                    print("The number for slots available for covishield is", random.randint(0, 50), "for today")
                    print("The cost of the vaccine is Rs.780")
                if page20 in ('2'):
                    print("The number for slots available for covaxin is", random.randint(0, 50), "for today")
                    print("The cost of the vaccine is Rs.780")
                if page19 in ('2'):
                    print("CHOOSE YOUR VACCINE:")
                    print("1.COVISHIELD")
                    print("2.COVAXIN")
                    page21 = input("ENTER YOUR INPUT(1/2)")
                    if page21 in ('1'):
                        print("The number of slots available for covishield is", random.randint(0, 40), "for today")
                        print("The cost of the vaccine is free")
                    if page21 in ('2'):
                        print("The number of slots available for covaxin is", random.randint(0, 40), "for today")
                        print("The cost of the vaccine is free")
                if page19 in ('3'):
                    print("CHOOSE YOUR VACCINE:")
                    print("1.COVISHIELD")
                    print("2.COVAXIN")
                    page22 = input("ENTER YOUR INPUT(1/2)")
                    if page22 in ('1'):
                        print("The number of slots available for covishield is", random.randint(0, 40), "for today")
                        print("The cost of the vaccine is free")
                    if page22 in ('2'):
                        print("The number of slots available for covaxin is", random.randint(0, 40), "for today")
                        print("The cost of the vaccine is free")
        if page18 in ('2'):
            print("1.VPS LAKESHORE HOSPITALS")
            print("2.ASTER MEDICITY")
            print("3.COCHIN GH")
            page23 = input("Enter your input(1/2/3):")
            if page23 in ('1'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page24 = input("ENTER YOUR INPUT(1/2/3):")
                if page24 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.2400")
                if page24 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.2000")
                if page24 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.2200")
            if page23 in ('2'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page25 = input("ENTER YOUR INPUT(1/2/3):")
                if page25 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.2400")
                if page25 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.2000")
                if page25 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.2200")
            if page23 in ('3'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page26 = input("ENTER YOUR INPUT(1/2/3):")
                if page26 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
                if page26 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
                if page26 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
        if page18 in ('3'):
            print("1.SIMANS HOSPITAL")
            print("2.KIIMS HOSPITAL")
            print("3.TRIVANDRUM GH")
            page27 = input("ENTER YOUR INPUT(1/2/3):")
            if page27 in ('1'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page28 = input("ENTER YOUR INPUT(1/2/3):")
                if page28 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 60), "for today")
                    print("The cost of the vaccine is 1600")
                if page28 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 60), "for today")
                    print("The cost of the vaccine is 1600")
                if page28 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 60), "for today")
                    print("The cost of the vaccine is 1600")
            if page27 in ("2"):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK V")
                page29 = input("ENTER YOUR INPUT(1/2/3):")
                if page29 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 60), "for today")
                    print("The cost of the vaccine is Rs.1600")
                if page29 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 60), "for today")
                    print("The cost of the vaccine is Rs.1600")
                if page29 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 60), "for today")
                    print("The cost of the vaccine is Rs.1600")
            if page27 in ("3"):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page29=input("ENTER YOUR INPUT(1/2/3):")
                if page29 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1600")
                if page29 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1600")
                if page29 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                    print("The cost of the vaccine is Rs.1600")
        if page18 in ('4'):
            print("CHOOSE YOUR HOSPITAL:")
            print("1.ELITE MISSION HOSPITAL")
            print("2.DAYA GENERAL HOSPITAL")
            print("3.THRISSUR GH")
            page31 = input("ENTER YOUR INPUT(1/2/3):")
            if page31 in ('1'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page32 = input("ENTER YOUR INPUT(1/2/3):")
                if page32 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1800")
                if page32 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1600")
                if page32 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                    print("The cost of the vaccine is Rs.1600")
            if page31 in ('2'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page33 = input("ENTER YOUR INPUT(1/2/3):")
                if page33 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1800")
                if page33 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1800")
                if page33 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                    print("The cost of the vaccine is Rs.1800")
            if page31 in ('3'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page34 = input("ENTER YOUR INPUT(1/2/3):")
                if page34 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
                if page34 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
                if page34 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                    print("The cost of the vaccine is free")
        if page18 in ('5'):
            print("1.NHIMS HOSPITALS")
            print("2.ALISTER MEDICAL CENTER")
            print("3.SHORNUR GH")
            page34 = input("ENTER YOUR INPUT(1/2/3):")
            if page34 in ('1'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page35 = input("ENTER YOUR INPUT(1/2/3):")
                if page35 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1800")
                if page35 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1600")
                if page35 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                    print("The cost of the vaccine is Rs.1600")
            if page34 in ('2'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page36 = input("ENTER YOUR INPUT(1/2/3):")
                if page36 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
                if page36 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
                if page36 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                    print("The cost of the vaccine is free")
            if page34 in ('3'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page37 = input("ENTER YOUR INPUT(1/2/3):")
                if page37 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
                if page37 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
    if page3 in ('3'):
        print("CHOOSE YOUR DISTRICT:")
        print("1.VIZAG")
        print('2.TIRUPATI')
        print('3.CHITTOOR')
        print('4.KURNOOL')
        print("5.SRIKAKULAM")
        page38 = input("ENTER YOUR INPUT(1/2/3/4/5):")
        if page38 in ('1'):
            print("CHOOSE YOUR HOSPITAL:")
            print("1.APOLLO HOSPITAL")
            print("2.VIZAG GH")
            page39 = input("ENTER YOUR INPUT(1/2):")
            if page39 in ('1'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                page40 = input("ENTER YOUR INPUT(1/2):")
                if page40 in ('1'):
                    print("The number for slots available for covishield is", random.randint(0, 50), "for today")
                    print("The cost of the vaccine is Rs.780")
                if page40 in ('2'):
                    print("The number for slots available for covaxin is", random.randint(0, 50), "for today")
                    print("The cost of the vaccine is Rs.780")
            if page39 in ('2'):
                    print("CHOOSE YOUR VACCINE:")
                    print("1.COVISHIELD")
                    print("2.COVAXIN")
                    page42 = input("ENTER YOUR INPUT(1/2)")
                    if page42 in ('1'):
                        print("The number of slots available for covishield is", random.randint(0, 40), "for today")
                        print("The cost of the vaccine is free")
                    if page42 in ('2'):
                        print("The number of slots available for covaxin is", random.randint(0, 40), "for today")
                        print("The cost of the vaccine is free")
        if page38 in ('2'):
            print("1.NARAYANDRI HOSPITALS")
            print("2.AMARAVATHI HOSPITAL")
            print("3.TIRUPATI GOVERNMENT GENRAL HOSPITAL")
            page43 = input("Enter your input(1/2/3):")
            if page43 in ('1'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page44 = input("ENTER YOUR INPUT(1/2/3):")
                if page44 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.2400")
                if page44 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.2000")
                if page44 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.2200")
            if page43 in ('2'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page45 = input("ENTER YOUR INPUT(1/2/3):")
                if page45 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.2400")
                if page45 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.2000")
                if page45 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.2200")
            if page43 in ('3'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page46 = input("ENTER YOUR INPUT(1/2/3):")
                if page46 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
                if page46 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
                if page46 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
        if page38 in ('3'):
            print("1.GLOBAL MULTISPECIALITY HOSPITAL")
            print("2.ESI HOSPITAL")
            print("3.CHITTOOR GH")
            page47 = input("ENTER YOUR INPUT(1/2/3):")
            if page47 in ('1'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page48 = input("ENTER YOUR INPUT(1/2/3):")
                if page48 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 60), "for today")
                    print("The cost of the vaccine is 1600")
                if page48 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 60), "for today")
                    print("The cost of the vaccine is 1600")
                if page48 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 60), "for today")
                    print("The cost of the vaccine is 1600")
            if page47 in ("2"):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page49 = input("ENTER YOUR INPUT(1/2/3):")
                if page49 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 60), "for today")
                    print("The cost of the vaccine is Rs.1600")
                if page49 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 60), "for today")
                    print("The cost of the vaccine is Rs.1600")
                if page49 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 60), "for today")
                    print("The cost of the vaccine is Rs.1600")
            if page47 in ("3"):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page50 = input("ENTER YOUR INPUT(1/2/3):")
                if page50 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1600")
                if page50 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1600")
                if page50 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                    print("The cost of the vaccine is Rs.1600")
        if page38 in ('4'):
            print("CHOOSE YOUR HOSPITAL:")
            print("1.OMNI HOSPITALS")
            print("2.MEDICARE HOSPITAL")
            print("3.KURNOOL GH")
            page51 = input("ENTER YOUR INPUT(1/2/3):")
            if page51 in ('1'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page52 = input("ENTER YOUR INPUT(1/2/3):")
                if page52 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1800")
                if page52 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1600")
                if page52 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                    print("The cost of the vaccine is Rs.1600")
            if page51 in ('2'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page53 = input("ENTER YOUR INPUT(1/2/3):")
                if page53 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1800")
                if page53 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1800")
                if page53 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                    print("The cost of the vaccine is Rs.1800")
            if page51 in ('3'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page54 = input("ENTER YOUR INPUT(1/2/3):")
                if page54 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
                if page54 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
                if page54 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                    print("The cost of the vaccine is free")
        if page38 in ('5'):
            print("1.MEDICOVER HOSPITAL")
            print("2.KIIMS HOSPITAL")
            print("3.SRIKULAM GH")
            page55 = input("ENTER YOUR INPUT(1/2/3):")
            if page55 in ('1'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page56 = input("ENTER YOUR INPUT(1/2/3):")
                if page56 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1800")
                if page56 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1600")
                if page56 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                    print("The cost of the vaccine is Rs.1600")
            if page55 in ('2'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page57 = input("ENTER YOUR INPUT(1/2/3):")
                if page57 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
                if page57 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
                if page57 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                    print("The cost of the vaccine is free")
            if page55 in ('3'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page58 = input("ENTER YOUR INPUT(1/2/3):")
                if page58 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
                if page58 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
                if page58 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                    print("The cost of the vaccine is free")
                print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                print("The cost of the vaccine is free")
    if page3 in ('4'):
        print("CHOOSE YOUR DISTRICT:")
        print("1.BANGALORE")
        print('2.MYSORE')
        print('3.MANGALORE')
        print('4.DHARWAD')
        print("5.BELAGAVI")
        page59 = input("ENTER YOUR INPUT(1/2/3/4/5):")
        if page59 in ('1'):
            print("CHOOSE YOUR HOSPITAL:")
            print("1.MANIPAL HOSPITAL")
            print("2.BANGALURU GH")
            page60 = input("ENTER YOUR INPUT(1/2):")
            if page60 in ('1'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                page61 = input("ENTER YOUR INPUT(1/2):")
                if page61 in ('1'):
                    print("The number for slots available for covishield is", random.randint(0, 50), "for today")
                    print("The cost of the vaccine is Rs.780")
                if page61 in ('2'):
                    print("The number for slots available for covaxin is", random.randint(0, 50), "for today")
                    print("The cost of the vaccine is Rs.780")
            if page60 in ('2'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                page62 = input("ENTER YOUR INPUT(1/2)")
                if page62 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 40), "for today")
                    print("The cost of the vaccine is free")
                if page62 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 40), "for today")
                    print("The cost of the vaccine is free")
        if page59 in ('2'):
            print("1.COLOUMBIA ASIA HOSPITAL")
            print("2.APOLLO HOSPITAL")
            print("3.MYSORE GOVERNMENT GENRAL HOSPITAL")
            page63 = input("Enter your input(1/2/3):")
            if page63 in ('1'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page64 = input("ENTER YOUR INPUT(1/2/3):")
                if page64 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.2400")
                if page64 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.2000")
                if page64 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.2200")
            if page63 in ('2'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page65 = input("ENTER YOUR INPUT(1/2/3):")
                if page65 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.2400")
                if page65 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.2000")
                if page65 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.2200")
            if page63 in ('3'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page66 = input("ENTER YOUR INPUT(1/2/3):")
                if page66 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
                if page66 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
                if page66 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
        if page59 in ('3'):
            print("1.HIGHLAND HOSPITAL")
            print("2.KMC HOSPITAL")
            print("3.MANGALORE GH")
            page67 = input("ENTER YOUR INPUT(1/2/3):")
            if page67 in ('1'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page68 = input("ENTER YOUR INPUT(1/2/3):")
                if page68 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 60), "for today")
                    print("The cost of the vaccine is 1600")
                if page68 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 60), "for today")
                    print("The cost of the vaccine is 1600")
                if page68 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 60), "for today")
                    print("The cost of the vaccine is 1600")
            if page67 in ("2"):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page69 = input("ENTER YOUR INPUT(1/2/3):")
                if page69 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 60), "for today")
                    print("The cost of the vaccine is Rs.1600")
                if page69 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 60), "for today")
                    print("The cost of the vaccine is Rs.1600")
                if page69 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 60), "for today")
                    print("The cost of the vaccine is Rs.1600")
            if page67 in ("3"):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page70 = input("ENTER YOUR INPUT(1/2/3):")
                if page70 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1600")
                if page70 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1600")
                if page70 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                    print("The cost of the vaccine is Rs.1600")
        if page59 in ('4'):
            print("CHOOSE YOUR HOSPITAL:")
            print("1.SPANDANA HOSPITALS")
            print("2.SHREEYA HOSPITALS")
            print("3.DHARWAD GH")
            page71 = input("ENTER YOUR INPUT(1/2/3):")
            if page71 in ('1'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page72 = input("ENTER YOUR INPUT(1/2/3):")
                if page72 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1800")
                if page72 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1600")
                if page72 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                    print("The cost of the vaccine is Rs.1600")
            if page71 in ('2'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page73 = input("ENTER YOUR INPUT(1/2/3):")
                if page73 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1800")
                if page73 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1800")
                if page73 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                    print("The cost of the vaccine is Rs.1800")
            if page71 in ('3'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page74 = input("ENTER YOUR INPUT(1/2/3):")
                if page74 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
                if page74 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
                if page74 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                    print("The cost of the vaccine is free")
        if page59 in ('5'):
            print("1.SUPER SPECIALITY HOSPITALS")
            print("2.YASH HOSPITAL")
            print("3.BELAGAVI GH")
            page75 = input("ENTER YOUR INPUT(1/2/3):")
            if page75 in ('1'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page76 = input("ENTER YOUR INPUT(1/2/3):")
                if page76 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1800")
                if page76 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is Rs.1600")
                if page76 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                    print("The cost of the vaccine is Rs.1600")
            if page75 in ('2'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page77 = input("ENTER YOUR INPUT(1/2/3):")
                if page77 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
                if page77 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
                if page77 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                    print("The cost of the vaccine is free")
            if page75 in ('3'):
                print("CHOOSE YOUR VACCINE:")
                print("1.COVISHIELD")
                print("2.COVAXIN")
                print("3.SPUTNIK")
                page78 = input("ENTER YOUR INPUT(1/2/3):")
                if page78 in ('1'):
                    print("The number of slots available for covishield is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
                if page78 in ('2'):
                    print("The number of slots available for covaxin is", random.randint(0, 100), "for today")
                    print("The cost of the vaccine is free")
                if page78 in ('3'):
                    print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                    print("The cost of the vaccine is free")
                print("The number of slots available for sputnik v is", random.randint(0, 40), "for today")
                print("The price of the vaccine is Rs.1600.")
if page1 in ('5'):
    print("1.COVISHIELD")
    print("2.COVAXINE")
    print("3.SPUTNIK V")
    page79=input("ENTER YOUR INPUT(1/2/3):")
    if page79 in ('1'):
        print("It is a recombinant, replication-deficient chimpanzee adenovirus vector encoding the SARS-CoV-2 Spike (S) glycoprotein.")
        print("Following administration, the genetic material of part of corona virus is expressed which stimulates an immune response.")
        print('This is also approved by World healt organisation(WHO)')
        print('Number of people vaccinated covishield in India are',random.randint(1000,10000000))
    if page79 in ('2'):
        print("Covaxin is an inactivated virus-based COVID-19 vaccine developed by Bharat Biotech in collaboration with the Indian Council of Medical Research.")
        print("Number of people vaccinated Covaxin in India are",random.randint(1000,10000000))
    if page79 in ('3'):
        print("The Russian Covid-19 vaccine Sputnik V (Gam-COVID-Vac) is an adenoviral-based, two-part vaccine.")
        print("Sputnik V uses a weakened virus to deliver small parts of a pathogen and stimulate an immune response.")
        print("Number of people vaccinated Covaxin in India are", random.randint(1000,10000000))
if page1 in ('6'):
    print("FOR ANY QUERY CONTACT:")
    print("TOLL FREE NO- 044-8967553")
    print("MAIL ID-mygov@gmail.com")
    print('*************JAI HIND**************')
