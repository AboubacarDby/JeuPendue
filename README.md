# JeuPendue
package fr.gouv.finances.exo;

import java.util.Scanner;

public class exercicePendue {

    public static void main(String[] args) {
	int i; // index mot pendue
	int nbEchec = 0;
	String motPendue;
	char alph;
	char[] tab;
	Scanner saisie = new Scanner(System.in);
	motPendue = saisie.nextLine();
	tab = new char[motPendue.length()];

	for (i = 0; i < motPendue.length(); i++) {
	    tab[i] = '_';

	}

	alph = saisie.nextLine().charAt(0);

	for (i = 0; i < tab.length; i++) {
	    if (motPendue.charAt(i) == alph) {
		tab[i] = alph;
	    }
	}

	// on va saisir un mot
	// donner une taille au tableau == mot
	// caractère saisie par le joueur
	// trouver le contenue
	// comparer alph avec chaque caractère du mot pendu
	saisie.close();

    }
}
