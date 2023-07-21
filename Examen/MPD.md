Hotels(<u>id</u>, nom)

Location(<u>(#id_chambre, #id_client)</u>)

Chambres(<u>id_chambre</u>, nom, disponible, prix_nuit, #id_hotel)

Entretenu(<u>(#id_chambre, #id_entretien)</u>, #id_chambre, #id_entretien)

Entretiens(<u>id_entretien</u>, date)

Realisation(<u>(#id_employe, #id_entretien)</u>, #id_entretien, #id_employe)

Forme(<u>(#id_employe, #id_formation)</u>, #id_formation, #id_employe)

Conges(<u>id_conge</u>, date_debut, date_fin, #id_employe)

Formations(<u>id_formation</u>, date_debut, date_fin)

Employes(<u>id_employe</u>, nom, prenom, adresse, ville, code_postal, #id_poste, #id_hotel)

Postes(<u>id_poste</u>, nom, heure_debut, heure_fin)

Tranferts(<u>id_transfert</u>, nom, date)

Recueille(<u>(#id_client, #id_hotel)</u>, #id_client, #id_hotel)

Clients(<u>id_client</u>, nom, prenom, adresse, ville, code_postal, #id_poste, #id_hotel)

Selection(<u>(#id_client, #id_service)</u>, #id_client, #id_service)

Services(<u>id_service</u>, #id_transfert, #id_activite)

Possession(<u>(#id_article, #id_hotel)</u>, #id_article, #id_hotel)

Articles(<u>id_article</u>, reference, prix)

Notes(<u>id_note</u>, score)

Notation(<u>(#id_note, #id_hotel, #id_client)</u>, #id_note, #id_hotel, #id_client)

Transactions(<u>id_transaction</u>,reference, total, #id_hotel, #id_facture)

Factures(<u>id</u>, reference, #id_hotel, #id_client)
Repas(<u>id</u>, nom)

Activites(<u>id</u>, nom, prix)

Compose(<u>(#id_repas, #id_plat)</u>, #id_plat, #id_repas)

Plats(<u>id</u>, nom, prix)




