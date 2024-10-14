import React from 'react';
import {Text, View, TextInput, Image} from 'react-native';

const Cat = () => {
  return <View style={{
    flex:1,
    justifyContent: 'center',
    alignItems: 'center',
    backgroundColor: '#ff5986'

  }}><Text>Hello, I am your Cat</Text></View>;
};

const Persona =() =>{
  const name="Darwin";
  return <View style={{
    flex:1,
    justifyContent: 'center',
    alignItems: 'center',
    backgroundColor: '#ff5986'
  }}><Text style={{
    color: '#74ffa2',
    fontFamily: 'Arial',
    fontStyle: 'ArialBlack',
    fontSize: 110,
    fontWeight: 20
  }}>Hello, I am {name}!</Text></View>;
};

const getFullName = (firstName: string, secondName:string, thirdName: string)=>{
  return firstName + ' '+ secondName+' '+ thirdName;
};

const Persona2 =()=>{
  return <View style={{
    flex:1,
    justifyContent: 'center',
    alignItems: 'center',
    backgroundColor: '#ff5986'
  }}><Text style={{
    color: '#74ffa2',
    fontFamily: 'Arial',
    fontStyle: 'ArialBlack',
    fontSize: 110,
    fontWeight: 20
  }}>Hello, I am  
  {getFullName('Rum', 'Tum', 'Tugger')}</Text></View>;
};
const Persona3 =()=>{
  return <View style={{
    flex:1,
    justifyContent: 'center',
    alignItems: 'center',
    backgroundColor: '#ff5986'
  }}><Text style={{
    color: '#74ffa2',
    fontFamily: 'Arial',
    fontStyle: 'ArialBlack',
    fontSize: 110,
    fontWeight: 20
  }}>Hello, I am... </Text><TextInput style={{
    height:40,
    borderColor:'gray',
    borderWidth:1}}
    defaultValue="Name me!"/> 
  </View>;
};

const Persona4 =props =>{
  return(
    <View style={{
    
    justifyContent: 'center',
    alignItems: 'center',
    backgroundColor: '#ff5986'
  }}><Text style={{
    color: '#74ffa2',
    fontFamily: 'Arial',
    fontStyle: 'ArialBlack',
    fontSize: 20,
    fontWeight: 20
  }}>Hello, I am  
  {props.name}</Text></View>
  );
}

const Cafe =()=>{
  return(
    <View>
    <Persona4 name="Darwin"/>
    <Persona4 name="Diego"/>
    <Persona4 name="Alberto"/>
    </View>
  )
}

const CatApp =()=>{
  return <View style={{
    flex:1,
    justifyContent: 'center',
    alignItems: 'center',
    backgroundColor: '#333333'
  }}><Image source={{uri:'https://media.tenor.com/PgAb0G8w_XEAAAAe/chomusuke-what.png'}} style={{width:200, height:200}}/><Text style={{
    color: '#c5c5c5',
    fontFamily: 'Arial',
    fontStyle: 'ArialBlack',
    fontSize: 100,
    fontWeight: 20
  }}>I am your cat</Text></View>;
}
export default CatApp;