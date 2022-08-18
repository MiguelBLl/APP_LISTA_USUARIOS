# APP_LISTA_USUARIOS
APLICACION REALIZADA POR EL GRUPO 1

import 'package:flutter/material.dart';

void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      theme: ThemeData(primarySwatch: Colors.lightGreen),
      home: Scaffold(
        appBar: AppBar(
          title: Text('ESPE-LATACUNGA'),
          leading: Image.network(
              'https://upload.wikimedia.org/wikipedia/commons/2/27/Logo_ESPE.png'),
        ),
        body: ListView(
          children: [
            Container(
              padding: EdgeInsets.symmetric(vertical: 10, horizontal: 50),
              child: ListTile(
                title: Text('Milber Beltran'),
                subtitle: Text('Director de ESPE-LATACUNGA'),
                leading: Image.network(
                    'https://espe-el.espe.edu.ec/wp-content/uploads/2022/05/TcrnDieloJimenez-220x3001-1.jpg'),
              ),
            ),
            Container(
              padding: EdgeInsets.symmetric(vertical: 10, horizontal: 50),
              child: ListTile(
                title: Text('Jorge Pardo'),
                subtitle:
                    Text('Director de Carrera Redes y Telecomunicaciones'),
                leading: Image.network(
                    'https://deee-el.espe.edu.ec/wp-content/uploads/2021/08/Jorge-Pardo3-230x307.jpg'),
                trailing: Icon(Icons.arrow_forward_ios),
              ),
            ),
            Container(
              padding: EdgeInsets.symmetric(vertical: 10, horizontal: 50),
              child: ListTile(
                title: Text('Javier Culqui'),
                subtitle: Text('Director de Carrera Electromecanica'),
                leading: Image.network(
                    'https://deee-el.espe.edu.ec/wp-content/uploads/2021/08/FOTO-JAVIER-CULQUI-350x353.jpg'),
                trailing: Icon(Icons.arrow_forward_ios),
              ),
            ),
            Container(
              padding: EdgeInsets.symmetric(vertical: 10, horizontal: 50),
              child: ListTile(
                title: Text('Pablo Pilatasig'),
                subtitle: Text('Director de Carrera Automatizacion'),
                leading: Image.network(
                    'https://deee-el.espe.edu.ec/wp-content/uploads/2021/08/PabloPilatasig-230x309.jpg'),
                trailing: Icon(Icons.arrow_forward_ios),
              ),
            ),
          ],
        ),
      ),
    );
  }
}
