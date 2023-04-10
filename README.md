# Caixa_eletr-nico-
Desenvolvimento de um caixa eletrônico funcional feito em Java Script

<html xmlns:mso="urn:schemas-microsoft-com:office:office" xmlns:msdt="uuid:C2F41010-65B3-11d1-A29F-00AA00C14882">

<head>

	<script>
		 
		 alert("Olá, bem vindo(a) ao nosso banco!");
		 var nome = prompt ("Por favor, informe o seu nome:");
		 parseInt (alert ("Olá " + nome + ", é um prazer ter você por aqui!"));
		 
		 var saldo = 532.5; 

		
		

		function inicio() {

			var escolha = parseInt(prompt('Selecione uma opção \n 1. Saldo \n 2.Extrato \n 3.Saque \n 4.Depósito \n 5.Tranferência \n 6.Sair'));

			
			switch (escolha) {
				case 1: ver_saldo();
					
					break;
				case 2: tirar_extrato();
					
					break;
				case 3: fazer_saque();
					
					break;
				case 4: fazer_deposito();
					
					break;
				case 5: fazer_tranferencia();
					
					break;
				case 6: sair();
					
					break;
				default: alert ("Escolha uma opção de acesso.");
				inicio ();
					break;
			}
		}		

		function ver_saldo() {
			
			var saldo = 532.5; 

			senha ();
			
			alert('Seu saldo atual é: R$' + saldo);
			
			inicio();
		}				

		function fazer_deposito() {
			var deposito = parseFloat(prompt('Qual o valor para depósito?'));
			// Not a Number
			if (isNaN(deposito) || deposito === '') {
				alert('Por favor, informe um número:');
				fazer_deposito();
			} else if (deposito <= 0) { não_autorizado ()

			} else {
				alert (deposito += saldo);
				inicio();				
			}
		}

		function fazer_saque() {

			
			senha ();
			var saque = parseFloat (prompt('Qual o valor para saque?'));

			if (isNaN(saque) || saque === '') {
				alert('Por favor, informe um número:');
				fazer_saque();
			
			} else if (saque > saldo) { alert ("Operação não autorizada.");


			}  else if (saque < 0 || saque == 0)
			{ não_autorizado ();
			
			} else { alert ("Saque realizado com sucesso! Veja seu saldo atual... ")
		}
			alert (saldo -= saque);
			inicio();
		}

		function tirar_extrato () {
					
					senha ();
					
					alert("27/02 - Pagamento  R$890 \n 03/03 - seguro cartao  R$77,90 \n 05/03 - int eletropaulo  R$108,83 \n 08/03 - rec bilhete unico sp  R$40,5 \n 15/03 - cinemark  R$137,30 \n 16/03 - extorno  R$ 7,03" );
						inicio();
					
		}

		function fazer_tranferencia () {
			 
			var saldo = 532.5; 


			senha();
			
			var conta = parseInt( prompt ("Informe o número da conta para qual deseja transferir.") );
				
			 

			 if (isNaN (conta) || conta == " " || conta <= 0) { alert ("Por favor, digite um número."); fazer_tranferencia();
						
					} else {  var valor = parseFloat (prompt ("Qual valor você deseja transferir?"));
									
					
				  

				}       var total = saldo - valor;
						alert("Transferência realizada com sucesso! \n Seu saldo atual é de R$ " + total);

						while (total > saldo) {
							alert("Operação não autorizada");
							fazer_transferencia();
						}
					
						 

							inicio();

		} 

			function senha () {
				const senha = parseFloat(prompt("Por favor, digite sua senha."));

				if (senha != 3589) { alert("Senha incorreta. Por favor, digite novamente");
				inicio ();
					}
			
			}



		function não_autorizado () {

			alert ("Operação não autorizada.")
		}

		function erro() {
			alert('Por favor, informe um número entre 1 e 6');
			inicio();
		}

		function sair() {
			var confirma = confirm('Você deseja sair?');

			if (confirma) { alert (nome + ", foi um prazer ter você conosco!");
				window.close();
			} else {
				inicio();
			}
		}

		
		
		inicio();
	</script>

<!--[if gte mso 9]><xml>
<mso:CustomDocumentProperties>
<mso:xd_Signature msdt:dt="string"></mso:xd_Signature>
<mso:display_urn_x003a_schemas-microsoft-com_x003a_office_x003a_office_x0023_Editor msdt:dt="string">GABRIEL AZEVEDO</mso:display_urn_x003a_schemas-microsoft-com_x003a_office_x003a_office_x0023_Editor>
<mso:Order msdt:dt="string">900.000000000000</mso:Order>
<mso:ComplianceAssetId msdt:dt="string"></mso:ComplianceAssetId>
<mso:TemplateUrl msdt:dt="string"></mso:TemplateUrl>
<mso:ReferenceId msdt:dt="string"></mso:ReferenceId>
<mso:xd_ProgID msdt:dt="string"></mso:xd_ProgID>
<mso:_ExtendedDescription msdt:dt="string"></mso:_ExtendedDescription>
<mso:display_urn_x003a_schemas-microsoft-com_x003a_office_x003a_office_x0023_Author msdt:dt="string">GABRIEL AZEVEDO</mso:display_urn_x003a_schemas-microsoft-com_x003a_office_x003a_office_x0023_Author>
<mso:TriggerFlowInfo msdt:dt="string"></mso:TriggerFlowInfo>
<mso:ContentTypeId msdt:dt="string">0x01010074B3227B3097A341A68CBB42830C4D3A</mso:ContentTypeId>
<mso:_SourceUrl msdt:dt="string"></mso:_SourceUrl>
<mso:_SharedFileIndex msdt:dt="string"></mso:_SharedFileIndex>
</mso:CustomDocumentProperties>
</xml><![endif]-->
<title></title></head>

<body>

</body>

</html>
