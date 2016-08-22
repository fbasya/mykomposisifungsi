
<!DOCTYPE html>
<html>
    <head></head>
    <body>
        <center>
            <br>
            <form name="tset">
                FUNGSI KOMPOSISI
                <br><br>
                Masukkan Fungsi Pertama f(x)<br><br>
                <input type="number" name="a1" id="a1" style="width:30px"> x<sup>2</sup> +
                <input type="number" name="b1" id="b1" style="width:30px"> x +
                <input type="number" name="c1" id="c1" style="width:30px"> <br><br>
                Masukkan Fungsi Pertama g(x)<br><br>
                <input type="number" name="a2" id="a2" style="width:30px"> x<sup>2</sup> +
                <input type="number" name="b2" id="b2" style="width:30px"> x +
                <input type="number" name="c2" id="c2" style="width:30px"> <br><br>
                <input type="button" name="f o g (x)" value="f o g (x)" onclick="myFunction()" ><br><br>
                <p> klik f o g untuk mengetahui pembahasannya</p>
                <p id="pembahasan"></p>
            </form>
            <script>
                function myFunction() {
                    var a1 = document.forms['tset']["a1"].value;
                    var b1 = document.forms['tset']["b1"].value;
                    var c1 = document.forms['tset']["c1"].value;
                    var a2 = document.forms['tset']["a2"].value;
                    var b2 = document.forms['tset']["b2"].value;
                    var c2 = document.forms['tset']["c2"].value;
                    var n1 = b1*a2;
                    var n2 = b1*b2;
                    var n3 = b1*c2;
                    var n4 = a2*a2;
                    var n5 = b2*b2;
                    var n6 = c2*c2;
                    var n7 = 2*a2*b2;
                    var n8 = 2*a2*c2;
                    var n9 = 2*b2*c2;
                    var n10 = n3+c1;
                    var n11 = a1*n4;
                    var n12 = a1*(n5+n8);
                    var n13 = a1*n6;
                    var n14 = a1*n7;
                    var n15 = a1*n9;
                    var n16 = (a1*b2*b2)+(a1*n8)+n1;
                    var n17 = n15+n2;
                    var n18 = n13+n3+c1;
                
                    document.getElementById("pembahasan").innerHTML ="<table>" + "<tr>" + "<td>" + "f &omicron; g (x)" + "</td>" + "<td>" + "= "+ a1 + "(" + a2 + "x<sup>2</sup> + " + b2 + "x + " + c2 + ")<sup>2</sup> +" + b1 + "(" + a2 + "x<sup>2</sup> + " + b2 + "x + " + c2 + ") +" + c1 + "</td>" + "</tr>" + "<tr>" + "<td>" + "  " + "</td>" + "<td>" + "= " + a1 + "[(" + a2 + "(x<sup>2</sup>))<sup>2</sup> + (" + b2 + "x)<sup>2</sup> + " + c2 + "<sup>2</sup> + 2(" + a2 + "x<sup>2</sup>)(" + b2 + "x) + 2(" + a2 + "x<sup>2</sup>)(" + c2 + ") + 2(" + b2 + "x)(" + c2 + ")] + " + n1 + "x<sup>2</sup> + " + n2 + "x + " + n3 + c1 + "</td>" + "</tr>" + "<tr>" + "<td>" + " " + "</td>" + "<td>" + "= "+ a1 + "[" + n4 + "x<sup>4</sup> + " + n5 + "x<sup>2</sup> + " + n6 + n7 + "x<sup>3</sup> + " + n8 + "x<sup>2</sup> +" + n9 + "x] + " + n1 + "x<sup>2</sup> + " + n2 + "x + " + n10 + "</td>" + "</tr>" + "<tr>" + "<td>" + " " + "</td>" + "<td>" + "= "+ a1 + "[" + n4 + "x<sup>4</sup> + (" + n5 + " + " + n8 + ") x<sup>2</sup> + " + n6 + "+ " + n7 + "x<sup>3</sup> +" + n9 + "x] + " + n1 + "x<sup>2</sup> + " + n2 + "x + " + n10 + "</td>" + "</tr>" + "<tr>" + "<td>" + " " + "</td>" + "<td>" + "= "+ n11 + "x<sup>4</sup> + " + n12 + "x<sup>2</sup> + " + n13 + "+ " + n14 + "x<sup>3</sup> +" + n15 + "x + " + n1 + "x<sup>2</sup> + " + n2 + "x + " + n10 + "</td>" + "</tr>" + "<tr>" + "<td>" + " " + "</td>" + "<td>" + "= "+ n11 + "x<sup>4</sup> + " + n14 + "x<sup>3</sup> + " + n12 + "x<sup>2</sup> " + n1 + "x<sup>2</sup> +" + n15 + "x + " + n2 + "x + " + n13 + " + " + n10 + "</td>" + "</tr>" + "<tr>" + "<td>" + " " + "</td>" + "<td>" + "= "+ n11 + "x<sup>4</sup> + " + n14 + "x<sup>3</sup> + " + n16 + "x<sup>2</sup> " + n17 + "x + "+
                n18 + "</td>" + "</tr>" + "</table><br>";}
                
            </script>
        </center>
    </body>
</html>
