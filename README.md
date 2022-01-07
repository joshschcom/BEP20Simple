# 1. Öffnen Sie Ihren Browser (in dem MetaMask konfiguriert ist) und navigieren Sie zuhttps://remix.ethereum.org

# 2. Sie können die Datei über diesen Gist-Link importieren . Sie können auch eine neue Datei mit dem Namen erstellen SampleBEP20Token.solund den oben angegebenen Code des BEP20-Token-Vertrags hinzufügen.

#3. Wir sollten unseren Code vor der Bereitstellung kompilieren. Durch Drücken der Ctrl + STasten wird der Code kompiliert. Sie können auch zur Kompilierungsseite navigieren, indem Sie auf die zweite Option im Navigationsbereich (ganz links) klicken.
Wir haben die Solidity-Version wie 0.8.4in unserem Code angegeben, daher müssen wir auch im Remix dieselbe Compiler-Version auswählen.

# 4. Nach erfolgreicher Kompilierung können Sie mit dem Bereitstellungsfenster fortfahren, indem Sie auf das Symbol unter dem Symbol „Compiler“ klicken.
Das ENVIRONMENTsollte so sein(JavaScript VM), Injected Web3wie wir MetaMask für die Bereitstellung verwenden. Stellen Sie außerdem sicher, dass Sie den SampleBEP20TokenVertrag in der CONTRACTDropdown-Liste (über der DeploySchaltfläche) ausgewählt haben.

Hinweis : Wir benötigen einige Testnetz-BNB, um das Gas während der Vertragserstellung zu bezahlen. Wir können Testnetz-BNB von diesem Wasserhahn erhalten. 

Wir sind alle bereit, unser SBT-Token bereitzustellen. Drücken Sie die DeployTaste. Es wird ein MetaMask-Popup zur Bestätigung ausgelöst. Klicken Sie hier Confirm, um das Token bereitzustellen. 

#5. Sobald die Transaktion abgeschlossen ist, werden die Protokolle sowie die Vertragsdetails unter dem Deployed ContractsAbschnitt angezeigt.

#6. Wenn wir auf die SAMPLEBEP20TOKENOption unter klicken, werden Depolyed Contractsdie öffentlichen Methoden und Variablen angezeigt, mit denen unsere Bereitstellung getestet werden kann. Lassen Sie uns den Kontostand des Vertragsinhabers überprüfen.
Jetzt können wir sehen, dass der Eigentümer / Administrator den erwarteten Gesamtvorrat des Tokens besitzt.

#7. Versuchen wir nun, die Token mit dieser transfer Methode in eine andere Brieftasche zu übertragen . Sobald der Empfänger addressund der amountzu sendende (mit einer Genauigkeit von 18) eingegeben wurden, klicken Sie auf die transferSchaltfläche. Es wird erneut ein Popup von der MetaMask angezeigt, in dem Sie zur Bestätigung der Transaktion aufgefordert werden. Beachten Sie, dass dieses Popup die Menge an Token enthält, die wir eingegeben haben.
Klicken Sie auf die ConfirmSchaltfläche, um die Transaktion zu verschieben. In wenigen Sekunden wird der Transaktionsstatus in den Remix-IDE-Protokollen angezeigt. Wir können den Transaktionsstatus auch im BSCScan Testnet Explorer überprüfen .
Wenn wir nun den Kontostand der Besitzer-Brieftasche erneut mit der balanceOfRemix-Methode überprüfen , sind es 10 Token weniger als eine Million.
Der Empfängerbrieftasche werden 10 SBT gutgeschrieben.
Jetzt können Sie so viele Token bereitstellen, wie Sie möchten. Das gleiche Verfahren kann zum Bereitstellen von Smartcontracts im BSC-Mainnet angewendet werden. Aber es wird Mainnet BNB für Gas kosten.

#8. *Hinzufügen unseres Tokens zu MetaMask*
         Klicken Sie auf die Add TokenSchaltfläche unten im ausgewählten MetaMask-Konto.
         Geben Sie die Vertragsadresse ein, die wir bereitgestellt haben. Das token nameund token symbolwird automatisch erkannt. Klicken Sie auf Next.
         Der Token-Kontostand des Kontos wird im nächsten Schritt angezeigt. Klicken Sie hier Add Tokens, um die Token zum MetaMask-Konto hinzuzufügen.
         Dieselbe Methode kann angewendet werden, um alle bereitgestellten Token im ausgewählten Netzwerk hinzuzufügen, in unserem Fall BSC Testnet.

 
