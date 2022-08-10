<h1 align="center"> 📘 Capitulo de Tratamento de erros</h1>

Conceitos e entendimentos do livro Clean Code - Resumo dissertativo 

indice 
<p align="center">
 <a href="#">Porque tratamento de erros?</a> •
 <a href="#"> Estrutura try-catch-finally</a> • 
 <a href="#">Null</a> • 

</p>

<h2 align="center"> 🔹 Porque tratamento de erros?</h2>
Tratamentos de erros são importantes porque toda tarefa ou codigo pode falhar. 
Porem excessos de tratamento de erros podem deixar o código confuso e dificil de entender

No livro ele menciona para retornar exceções de vez codigos. Retornar uma exceção seria retornar o erro que esta causando.
```
public void sendShutDown(){
  try{
    tryToShutDown();
  } catch (DeviceShutDownError e){
    logger.log(e);
  }
}
private void tryToShutDown() thorows DeviceShutDownError{
  DeviceHandle handle -= getHandle e (DEVl);
  DeviceRecord record = retrieveDeviceRecord(handle);

  pauseDevice (handle);
  clearDeviceWorkQueue (handle);
  closeDevice (handle);
}
private DeviceHandle getHandle(DeviceID id) {
  throw new DeviceShutDownError("Invalid handle for: " + id.toString())
}
```

<h2 align="center"> 🔹 Estrutura try-catch-finally</h2>
try - parte que executa o código 
catch - tem que retornar a exceção a parte do erro
finally - retonar a função ou finaliza o processo

<h2 align="center"> 🔹Exceçoes com contexto</h2>

Forneca exceçoes com contexto para determinar de fato o problema.
Evite mensagens como "Deu erro", mencione a operação que falou e o tipo da falha.

Da para definir e classificar tipos de erros e assim informara origem, se veio de um componente ou dispositivo.

<h2 align="center"> 🔹Null</h2>

Não retorne no seu tratamento de erros , null ou não use null como parametro. 
Retornar null vc esta se dando um retrabalho de verificação 
Ao inves de retornar null tente trazer uma exceção do problema.
### Breve entendimento do capitulo 7 do capitulo do livro clean code