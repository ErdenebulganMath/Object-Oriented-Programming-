// Амьдрал дээр байгаа объектуудыг (шинж чанартай, үйл хөдөлөлтэй юмыг хэлдэг)
// програмчлалын хэл дээр хэрхэн загварчлах талаар жишээ код.
// Ажилчин классыг загварчилсан ба дараах шинж чанар, үйл хөдлөлтэй байна:
// Шинж чанар: нэр, албан тушаал, цалин, заадаг хичээл. Эдгээр нь классын гишүүн өгөгдөл болно.
// Үйл хөдлөл: хичээл заах, ажиллах, цалин авах. Эдгээр нь классын гишүүн функц болно.
#include <iostream>
using namespace std;
// Ажилтныг загварчилсан класс буюу үүсмэл өгөгдлийн төрөл зарлаж байна. class түлхүүр үг ашиглана
class Employee {
public:
    // гишүүн өгөгдлүүд буюу ажилтны шинж чанарыг зарлаж байна
    char name[50];
    char position[50];
    float salary;
    char course_name[50];
    // гишүүн функцүүд буюу үйл хөдлөл (behaviour) зарлаж байна
    int teach();
    int work();
    float get_salary();
};
// Гишүүн функцүүдийг классын гадна талд тодорхойлж байна
int Employee::teach(){
    // Гишүүн функц нь гишүүн өгөгдөлд шууд хандах боломжтой. Энд name, course_name нэртэй өгөгдлүүдэд хандаж байна.
    cout<<name<<" is teaching "<<course_name<<endl;
}
int Employee::work(){
    // Гишүүн функц нь өөр нэг гишүүн функцийг дуудаж болно. Энд get_salary функцийг дуудаж байна.
    cout<<name<<" is working as "<<position
    << " and for salary "<<get_salary()<<endl;
}
float Employee::get_salary(){
    // Гишүүн функц нь гишүүн өгөгдөлд хандах боломжтой
    cout<<name<<" is getting "<<salary<<" as salary"<<endl;
    return salary;
}
int main(){
    int n; // n хувьсагч бол instance буюу int төрлөөс үүссэн бодит хувьсагч
    Employee bat, dorj; //bat хувьсагч бол instance буюу Employee төрлөөс үүссэн объект юм
    
    // Классын гишүүн өгөгдөлд объектээр дамжуулж хандана. Employee.name гэж болохгүй. bat.salary = 2000; гэж болно
    strcpy(bat.name, "Bat");
    strcpy(bat.position, "Lecturer");
    bat.salary=2000;
    strcpy(bat.course_name, "C++ Programming");
    
    // Классын гишүүн функцийг объектээр дамжуулж дуудна.
    bat.teach();
    bat.work();
    cout<<"Bat's salary: "<<bat.get_salary()<<endl;

    strcpy(dorj.name, "Dorj");
    strcpy(dorj.position, "Lecturer");
    dorj.salary=3000;
    strcpy(dorj.course_name, "Java Programming");
    dorj.teach();
    dorj.work();
    cout<<"Dorj's salary:"<<dorj.get_salary()<<endl;
} 
