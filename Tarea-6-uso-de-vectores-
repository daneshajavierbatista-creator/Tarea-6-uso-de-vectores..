#include <iostream>
#include <vector>
using namespace std;

struct Producto {
    string nombre;
    float precio;
};

int main() {
    vector<Producto> inventario = {
        {"Arroz", 75}, {"Leche", 65}, {"Pan", 45},
        {"Huevos", 120}, {"Cafe", 180}
    };

    inventario.push_back({ "Azucar", 80 });

    for (auto p : inventario)
        cout << p.nombre << " - $" << p.precio << endl;

    inventario[0].precio = 90;

    float suma = 0;
    for (auto p : inventario) suma += p.precio;

    cout << "\nPromedio: $" << suma / inventario.size() << endl;
    cout << "Primer producto: " << inventario.at(0).nombre << endl;

    Producto mayor = inventario[0];
    for (auto p : inventario)
        if (p.precio > mayor.precio) mayor = p;

    cout << "Mas caro: " << mayor.nombre << " - $" << mayor.precio;

    return 0;
}
