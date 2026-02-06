# tareas-de-SO
#include <iostream>
#include <fstream>

using namespace std;

int main() {
    ofstream archivo;
    archivo.open("archivo.txt");
    archivo << "Hola mundo";
    archivo.close();

    ifstream archivoLectura;
    string texto;
    archivoLectura.open("archivo.txt");
    archivoLectura >> texto;
    cout << texto << endl;
    archivoLectura.close();

    return 0;
}
