# AppBlaBlaCar
package com.example.replicablablacaroficial
import android.annotation.SuppressLint
import androidx.compose.foundation.background
import androidx.compose.foundation.layout.Arrangement
import androidx.compose.foundation.layout.Box
import androidx.compose.foundation.layout.Column
import androidx.compose.foundation.layout.Row
import androidx.compose.foundation.layout.Spacer
import androidx.compose.foundation.layout.fillMaxHeight
import androidx.compose.foundation.layout.fillMaxSize
import androidx.compose.foundation.layout.fillMaxWidth
import androidx.compose.foundation.layout.height
import androidx.compose.foundation.layout.padding
import androidx.compose.foundation.layout.size
import androidx.compose.foundation.layout.width
import androidx.compose.material.icons.Icons
import androidx.compose.material.icons.filled.AccountCircle
import androidx.compose.material.icons.filled.AddCircle
import androidx.compose.material.icons.filled.CheckCircle
import androidx.compose.material.icons.filled.Face
import androidx.compose.material.icons.filled.KeyboardArrowRight
import androidx.compose.material.icons.filled.List
import androidx.compose.material.icons.filled.MailOutline
import androidx.compose.material.icons.filled.Search
import androidx.compose.material3.Button
import androidx.compose.material3.Card
import androidx.compose.material3.Icon
import androidx.compose.material3.IconButton
import androidx.compose.material3.Scaffold
import androidx.compose.material3.Surface
import androidx.compose.material3.Text
import androidx.compose.runtime.Composable
import androidx.compose.ui.Alignment
import androidx.compose.ui.Modifier
import androidx.compose.ui.graphics.Color
import androidx.compose.ui.text.font.FontWeight
import androidx.compose.ui.tooling.preview.Preview
import androidx.compose.ui.unit.dp
import androidx.compose.ui.unit.sp
import androidx.compose.material3.CardDefaults
import androidx.compose.material3.Divider



@SuppressLint("UnusedMaterial3ScaffoldPaddingParameter")
@Preview
@Composable

fun TelaPerfil () {
    Scaffold(
        modifier = Modifier.height(750.dp)
    ) {
        Column(
            modifier = Modifier

                .fillMaxWidth()
                .height(750.dp)
                .background(color = Color.White))
        {
            Menuu()
            Cardone()
            Cardduo()
            Cartry()
            CarFor()
            CarFive()
            MenuInferior()
        }
    }
}

@Composable
fun Cardone() {

    Card(
        modifier = Modifier
            .fillMaxWidth()
            .height(100.dp)
            .padding(0.dp, 10.dp)
            .background(color = Color.White)
    ) {Divider(modifier = Modifier.padding(vertical = 2.dp).weight(5f))
        Row()
        {
            Box(
                modifier = Modifier
                    .fillMaxHeight()
                    .weight(2f)
                    .background(color = Color.White)


            ) {
                Icon(
                    imageVector = Icons.Filled.AccountCircle,
                    contentDescription = "Ícone do Perfil",
                    modifier = Modifier
                        .fillMaxSize()
                )
            }
            Box(
                modifier = Modifier
                    .fillMaxHeight()
                    .weight(5f)


            ) {

                Column(
                    modifier = Modifier
                        .fillMaxSize()
                        .background(color = Color.White),
                    verticalArrangement = Arrangement.Center
                )
                {

                    Text("Northon", fontSize = 25.sp, fontWeight = FontWeight.Bold)

                    Text("Principiante",fontWeight = FontWeight.Bold, color = Color.Gray)
                }
            }
            Box(
                modifier = Modifier
                    .fillMaxHeight()
                    .weight(2f)
                    .background(color = Color.White),
                contentAlignment = Alignment.CenterEnd


            ) {
                IconButton(
                    onClick = {}
                ) {
                    Icon(
                        imageVector = Icons.Filled.KeyboardArrowRight,
                        contentDescription = "Ícone do Perfil",
                        modifier = Modifier.size(30.dp),
                        tint = Color.Gray



                    )
                }
            }


        }
    }
}
@Composable
fun Menuu (){
    Surface(
        modifier = Modifier
            .fillMaxWidth()
            .height(50.dp))
    {
        Row()
        {
            Box(
                modifier = Modifier
                    .fillMaxSize()
                    .background(color = Color.White)
                    .weight(5f))
            {
                Button(
                    onClick = {},
                    modifier = Modifier
                        .fillMaxSize(),
                    colors = androidx.compose.material3.ButtonDefaults
                        .buttonColors(Color.White))
                {
                    Text("Sobre você", color = Color.Black)
                }
            }
            Box(
                modifier = Modifier
                    .fillMaxSize()
                    .background(color = Color.White)
                    .weight(5f))
            {
                Button(
                    onClick = {},
                    modifier = Modifier
                        .fillMaxSize(),
                    colors = androidx.compose.material3.ButtonDefaults
                        .buttonColors(Color.White)
                ) {
                    Text("Conta", color = Color.Black)
                }
            }

        }
    }
}

@Composable
fun Cardduo(){
    Card(
        colors = CardDefaults.cardColors(Color(0xFF8FFCBD)),
        modifier = Modifier
            .height(100.dp)
            .fillMaxWidth()
            .padding(10.dp)
    ) {

        Column (
            modifier = Modifier
                .padding(10.dp)
                .fillMaxWidth(),

        ) {



            Spacer(modifier = Modifier.width(20.dp))

            Column {
                Text("Desde que se juntou á BlablaCar, você economizou", fontWeight = FontWeight.Bold,fontSize = 15.sp)
                Text("R$ 115",fontWeight = FontWeight.Bold, fontSize = 30.sp, color = Color(
                    0xFF009D35
                )
                )
            }

        }

    }
}

@Composable
fun Cartry(){
    Card(
        colors = CardDefaults.cardColors(Color(0xFFA3E6FD)),
        modifier = Modifier
            .height(160.dp)
            .fillMaxWidth()
            .padding(10.dp)
    ) {

        Column (
            modifier = Modifier
                .padding(10.dp)
                .fillMaxWidth(),

            ) {
            Text("Comprete seu perfil", fontWeight = FontWeight.Bold, fontSize = 20.sp)
            Text("Isso ajuda a construir confiança, incentivando os menbros a viajarem com vcoê."
                ,fontWeight = FontWeight.Bold, fontSize = 15.sp, color = Color.Black,
                modifier = Modifier .padding(0.dp,10.dp)
            )

            Row() {
                Box (modifier = Modifier
                    .padding(7.dp, 0.dp)
                    .background(color = Color(0xFF0090FF))
                    .height(5.dp)
                    .width(45.dp)){}
                Box (modifier = Modifier
                    .padding(7.dp, 0.dp)
                    .background(color = Color(0xFF0090FF))
                    .height(5.dp)
                    .width(45.dp)){}

                Box (modifier = Modifier
                    .padding(7.dp, 0.dp)
                    .background(color = Color(0xFF0090FF))
                    .height(5.dp)
                    .width(45.dp)){}

                Box (modifier = Modifier
                    .padding(7.dp, 0.dp)
                    .background(color = Color(0xFF0090FF))
                    .height(5.dp)
                    .width(45.dp)){}

                Box (modifier = Modifier
                    .padding(7.dp, 0.dp)
                    .background(color = Color.White)
                    .height(5.dp)
                    .width(45.dp)){}

                Box (modifier = Modifier
                    .padding(7.dp, 0.dp)
                    .background(color = Color.White)
                    .height(5.dp)
                    .width(45.dp)){}
            }
            Text("Adicionar preferência de viagem."
                ,fontWeight = FontWeight.Bold, fontSize = 15.sp, color = Color(0xFF0090FF),
                modifier = Modifier .padding(0.dp,10.dp))




        }

    }
}

@Composable
fun CarFor(){
    Card(
        colors = CardDefaults.cardColors(Color.White),
        modifier = Modifier

            .padding(10.dp)
    ) {
        Text("Modificar foto de perfil", fontWeight = FontWeight.Bold, color = Color(0xFF0090FF),fontSize = 14.sp,
            modifier = Modifier.padding(8.dp)
        )

        Text("Modificar dados pessoais", fontWeight = FontWeight.Bold, color = Color(0xFF0090FF), fontSize = 14.sp,
            modifier = Modifier.padding(8.dp,0.dp))


        }
    Divider(modifier = Modifier.padding( 10.dp))
    }


@Composable
fun CarFive(){
    Card(
        colors = CardDefaults.cardColors(Color.White),
        modifier = Modifier
            .height(180.dp)
            .fillMaxWidth()
            .padding(10.dp)
    ) {

        Column (
            modifier = Modifier

                .fillMaxWidth(),

            ) {
            Text("Você tem um Pefil Verificado", fontWeight = FontWeight.Bold,
                fontSize = 20.sp,modifier = Modifier .padding(3.dp,0.dp))

            Row(
                modifier = Modifier
                    .fillMaxWidth()
                    .background(color = Color.White)
                    .padding(0.dp, 10.dp)
            ){
                Icon(
                imageVector = Icons.Filled.CheckCircle,
                contentDescription = "Ícone do Perfil",
                modifier = Modifier
                    .size(25.dp)
                    .padding(0.dp, 2.dp, 10.dp)
                    .weight(1f),
                tint = Color(0xFF0090FF))

                Text("Documentação confirmada."
                    ,fontWeight = FontWeight.Bold, fontSize = 14.sp, color = Color.Black,
                    modifier = Modifier
                        .padding(0.dp, 6.dp)
                        .weight(8f))



            }
            Row(
                modifier = Modifier
                    .fillMaxWidth()
                    .background(color = Color.White)
                    .padding(0.dp)
            ){
                Icon(
                    imageVector = Icons.Filled.CheckCircle,
                    contentDescription = "Ícone do Perfil",
                    modifier = Modifier
                        .size(25.dp)
                        .padding(0.dp, 2.dp, 10.dp)
                        .weight(1f),
                    tint = Color(0xFF0090FF))
                Text("Northon@gmai.com."
                    ,fontWeight = FontWeight.Bold, fontSize = 14.sp, color = Color.Black,
                    modifier = Modifier
                        .padding(0.dp, 6.dp)
                        .weight(8f))
            }
            Row(
                modifier = Modifier
                    .fillMaxWidth()
                    .background(color = Color.White)
                    .padding(0.dp, 10.dp)
            ){
                Icon(
                    imageVector = Icons.Filled.CheckCircle,
                    contentDescription = "Ícone do Perfil",
                    modifier = Modifier
                        .size(25.dp)
                        .padding(0.dp, 2.dp, 10.dp)
                        .weight(1f),
                    tint = Color(0xFF0090FF))

                Text("+5541999999999."
                    ,fontWeight = FontWeight.Bold, fontSize = 14.sp, color = Color.Black,
                    modifier = Modifier
                        .padding(0.dp, 6.dp)
                        .weight(8f))



            }

        }


    }
    Divider(modifier = Modifier.padding(vertical = 2.dp))

}
@Composable
fun MenuInferior(){
        Surface(
        modifier = Modifier
        .fillMaxWidth()
        .height(50.dp))
        {
            Row()
            {
                Box(
                    modifier = Modifier
                        .fillMaxSize()
                        .background(color = Color.White)
                        .weight(2f))
                {
                    Button(
                        onClick = {},
                        modifier = Modifier
                            .fillMaxSize(),
                        colors = androidx.compose.material3.ButtonDefaults
                            .buttonColors(Color.White))
                    {
                        Icon(
                            imageVector = Icons.Filled.Search,
                            contentDescription = "Ícone do Perfil",
                            modifier = Modifier
                                .size(30.dp)

                                .weight(1f),
                            tint = Color(0xFF0090FF))
                    }
                }
                Box(
                    modifier = Modifier
                        .fillMaxSize()
                        .background(color = Color.White)
                        .weight(2f))
                {
                    Button(
                        onClick = {},
                        modifier = Modifier
                            .fillMaxSize(),
                        colors = androidx.compose.material3.ButtonDefaults
                            .buttonColors(Color.White)
                    ) {
                        Icon(
                            imageVector = Icons.Filled.AddCircle,
                            contentDescription = "Ícone do Perfil",
                            modifier = Modifier
                                .size(30.dp)

                                .weight(1f),
                            tint = Color(0xFF0090FF))
                    }
                }
                Box(
                    modifier = Modifier
                        .fillMaxSize()
                        .background(color = Color.White)
                        .weight(2f))
                {
                    Button(
                        onClick = {},
                        modifier = Modifier
                            .fillMaxSize(),
                        colors = androidx.compose.material3.ButtonDefaults
                            .buttonColors(Color.White)
                    ) {
                        Icon(
                            imageVector = Icons.Filled.List,
                            contentDescription = "Ícone do Perfil",
                            modifier = Modifier
                                .size(30.dp)

                                .weight(1f),
                            tint = Color(0xFF0090FF))
                    }
                }
                Box(
                    modifier = Modifier
                        .fillMaxSize()
                        .background(color = Color.White)
                        .weight(2f))
                {
                    Button(
                        onClick = {},
                        modifier = Modifier
                            .fillMaxSize(),
                        colors = androidx.compose.material3.ButtonDefaults
                            .buttonColors(Color.White)
                    ) {
                        Icon(
                            imageVector = Icons.Filled.MailOutline,
                            contentDescription = "Ícone do Perfil",
                            modifier = Modifier
                                .size(30.dp)

                                .weight(1f),
                            tint = Color(0xFF0090FF))
                    }
                }
                Box(
                    modifier = Modifier
                        .fillMaxSize()
                        .background(color = Color.White)
                        .weight(2f))
                {
                    Button(
                        onClick = {},
                        modifier = Modifier
                            .fillMaxSize(),
                        colors = androidx.compose.material3.ButtonDefaults
                            .buttonColors(Color.White)
                    ) {
                        Icon(
                            imageVector = Icons.Filled.Face,
                            contentDescription = "Ícone do Perfil",
                            modifier = Modifier
                                .size(30.dp)

                                .weight(1f),
                            tint = Color(0xFF0090FF))
                    }
                }
            }
        }
}






