# Paid# طلب المعلومات من المستخدم
name = input("من فضلك، أدخل اسمك: ")
age = input("كم عمرك؟ ")

# اسم الملف الذي سنقوم بالحفظ فيه
file_name = "user_info.txt"

# فتح الملف في وضع الكتابة (append) لإضافة سطر جديد دون مسح المحتوى القديم
with open(file_name, "a", encoding="utf-8") as file:
    # كتابة المعلومات في الملف
    file.write(f"الاسم: {name}\n")
    file.write(f"العمر: {age}\n")
    file.write("-" * 20 + "\n")  # إضافة خط فاصل

print(f"تم حفظ المعلومات بنجاح في ملف {file_name}.")
