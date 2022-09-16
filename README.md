# latihan_frontendsyahira
this is my first repository in github
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
    <link rel="stylesheet" href="DataTables/datatables.min.css">
</head>
<body>
    <table id="contoh" class="display">
        <thead>
            <tr>
                <th width=10%>NO</th>
                <th width=50%>Nama</th>
                <th width=15%>Kelas</th>
                <th width=15%>Alamat</th>
                <th width=15%>No HP</th>
            </tr>
        </thead>
    </table>
    <script src="DataTables/jQuery-3.6.0/jquery-3.6.0.min.js"></script>
    <script src="DataTables/datatables.min.js"></script>
    <script>
        $(function(){
            //var data = [
            //    ["1","Udin","1","alamat","087720008578"]
            //    ["2","Samsudin","2","alamat","087720008578"]
            //    ];
            var data =[];
            for (let i = 0; i < 50; i++){
                data.push([i]);
                for (let j = 0; j < 50; j++){
                    data[i].push(j);
                }
            }
            $("#contoh").DataTable({
                responsive : true,
                data : data
            });
        });
    </script>
</body>
</html>
