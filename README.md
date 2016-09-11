# ATMelso
ATM tombok nelkul
 public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int penz = 0;

        System.out.print("Mennyi pénzt szeretnél felvenni?: ");
        penz = sc.nextInt();

        if (0 < penz && penz <= 250000) {
            System.out.println("Kapsz: ");
            int huszezres = penz / 20000;
            penz = penz % 20000;
            if (huszezres > 0) {
                System.out.println(huszezres + " darab húszezrest, ");
            }
            if (penz > 0) {
                int tizezres = penz / 10000;
                penz = penz % 10000;

                if (tizezres > 0) {
                    System.out.println(tizezres + " darab tízezrest, ");
                }
                if (penz > 0) {
                    int otezres = penz / 5000;
                    penz = penz % 5000;

                    if (otezres > 0) {
                        System.out.println(otezres + " darab ötezrest, ");
                    }
                    if (penz > 0) {
                        int ketezres = penz / 2000;
                        penz = penz % 2000;

                        if (ketezres > 0) {
                            System.out.println(ketezres + " darab kétezrest, ");
                        }
                        if (penz > 0) {
                            int ezres = penz / 1000;
                            penz = penz % 1000;
                            if (ezres > 0) {
                                System.out.println(ezres + " darab ezrest, ");
                            }
                            if (penz > 0) {
                                int otszazas = penz / 500;
                                penz = penz % 500;

                                if (otszazas > 0) {
                                    System.out.println(+otszazas + "darab ötszázast, ");
                                }
                                if (penz > 0) {
                                    int ketszazas = penz / 200;
                                    penz = penz % 200;

                                    if (ketszazas > 0) {
                                        System.out.println(ketszazas + " darab kétszázast, ");
                                    }
                                    if (penz > 0) {
                                        int szazas = penz / 100;
                                        penz = penz % 100;

                                        if (szazas > 0) {
                                            System.out.println(szazas + " darab százast, ");
                                        }
                                        if (penz > 0) {
                                            int otvenes = penz / 50;
                                            penz = penz % 50;

                                            if (otvenes > 0) {
                                                System.out.println(otvenes + " darab ötvenest, ");
                                            }
                                            if (penz > 0) {
                                                int huszas = penz / 20;
                                                penz = penz % 20;

                                                if (huszas > 0) {
                                                    System.out.println(huszas + " darab huszast, ");
                                                }
                                                if (penz > 0) {
                                                    int tizes = penz / 10;
                                                    penz = penz % 10;

                                                    if (tizes > 0) {
                                                        System.out.println(tizes + " darab tizest, ");
                                                    }
                                                    if (penz > 0) {
                                                        int otos = penz / 5;
                                                        penz = penz % 5;

                                                        if (otos > 0) {
                                                            System.out.println(otos + " darab ötforintost, ");
                                                        }
                                                    }
                                                }
                                            }
                                        }
                                    }
                                }
                            }
                        }
                    }
                }
            }
        } else {
            System.out.println("A minimum összeg 0, a maximum 250000!");
        }
    }
}
