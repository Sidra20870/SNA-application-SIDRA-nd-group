<!DOCTYPE html>
<html>
<head>
</head>
<body>
     <div style="background-color:black;color:white;padding:20px;">
          <h1> DM 103348: Graph theory using SNA (social network analysis) </h1>
     <h3> Project Members </h3>
          <table style="width:100%">
  <tr>
    <th>Student Id</th>
    <th>Student Name</th> 
  </tr>
  <tr>
       <td><b>63986</b></td>
       <td><b>Sidra Usman(leader)</b></td>
  </tr>
  <tr>
    <td>63813</td>
    <td>Muhammad Ammar Haider</td>
  </tr>
  <tr>
    <td>63650</td>
    <td>Dua Javeria</td>
  </tr>
  <tr>
    <td>63814</td>
    <td>Muhammad Saqlain</td>
  </tr>
  <tr>
    <td>63761</td>
    <td>Humaira Noor</td>
  </tr>
            
</table>

<h2> Project Description </h2>
<p style="background-color:Tomato;"> SNA: Network is a bundle of modules for network algorithms, specifically designed for the needs of Social Network Analysis (SNA), but can be used for any other graph algorithms. It represents a standard directed and weighted network, which can also be used as an undirected and/or unweighted network of course.
We are looking forward to get a social data and find the relationship between the people using SNA graph theory concept 
Relationship includes,knowing a user which is connected to maximum or minimum number of other users, mutual connections, connection of each employee etc.
</p>

<h2>Discrete Math Concepts Used </h2>
<ul>
     <li>*Graph theory using social network analysis</li>
     <li>*Analyze any data from network social media</li>
     <li>*Long time existence</li>
     <li>*Mapping :</li>
     <ul>
          <li> * Relation or information between</li>
          <ul>
               <li>* People</li>
               <li>* Team </li>
               <li>* Organization</li>
          </ul>
     </ul>
</ul>

 <div>
    </p>
     <center><h2>MENU</h2></center>
     <p>
          print('press 1 to get number of nodes')<br>
          print('press 2 to get number of edges')<br>
          print('press 3 to get number of connected nodes')<br>
          print('press 4 to draw graph')<br>
          print('press 5 to get  path')<br>
          print('press 6 to shortest path ')<br>
          print('press 7 to get information')<br>
          print('press 8 to get triadic closure')<br>
          print('press 9 to get SELF CONNECTED PEOPLE')<br>
          print('press 10 to get most connected person')<br>
          print('press 11 to get mutual connections')
     </p>
         
</div>
<h2>CODE</h2>
<div>
     <p>
          import networkx as nz<br>
          G_symmetric = nz.Graph()<br>
          G_fb = nz.read_edgelist('facebook_combined.txt', create_using = nz.Graph(), nodetype=str)<br>
          ch=input('enter your choice')
          <hr>
          if ch=='3':<br>
          count=0<br>
          nodee=input('enter the node')<br>
          for n in G_fb.neighbors(nodee):<br>
            print(n)<br>
            count+=1<br>
          print("no.of edges=",count)
          <hr>
     if ch=='10': <br>
    li=[]<br>
    maxx=0<br>
    mn=0<br>
    minnode=0<br>
    minn=10<br>
    for i in G_fb:<br>
        li=list(nz.neighbors(G_fb,i))<br>
        if(maxx<len(li)):<br>
            maxx=len(li)<br>
            mn=i<br>
        if(minn>len(li)):<br>
            minn=len(li)<br>
            minnode=i<br>
    print("PERSON= "+str(mn)+"  connections= "+str(maxx))<br>
    print("PERSON= "+str(minnode)+"  connections= "+str(minn))
     <hr>
     if ch=='11':<br>
    p1=input("person A?")<br>
    p2=input("person B?")<br>
    print('MUTUAL CONNECTIONS')<br>
    print(sorted(nz.common_neighbors(G_fb, p1,p2)))
   
          
    
 </div>
<h2> Problem Faced </h2>
<p>We have use networkx(library) built-in functions which were very difficult to understand but with the help of internet and understand their meta data and overcome this problem. We were facing communication problem among project partners beside this, this library contain limit functions which cause us to think how to distribute functions between the partners. So we decided each partner will do 2-3 functions
  

we never had an experince of importing any social organization data into our project.finding and importing data took our huge time. 
</p>
<h2> References </h2>
https://networkx.github.io/documentation/stable/reference/functions.html<br>
https://www.datacamp.com/community/tutorials/social-network-analysis-python<br>
https://www.python-course.eu/graphs_python.php<br>
https://metacpan.org/pod/SNA::Network

</div>

</body>
</html>
