import matplotlib.pyplot as plt

# 1) Урожайність зернових (2013–2022)
years_yield = [2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022]
yield_values = [86.3, 90.7, 87.5, 77.8, 87.9, 79.1, 86.5, 79.2, 78.7, 89.4]

plt.figure()
plt.plot(years_yield, yield_values, marker='o')
plt.title("Урожайність зернових і зернобобових культур (ц/га)")
plt.xlabel("Рік")
plt.ylabel("ц/га")
plt.grid(True)
plt.savefig("yield_cereals.png", bbox_inches="tight")
plt.close()

# 2) Покриття імпорту експортом (2015–2024)
years_trade = [2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023, 2024]
coverage_values = [1.100, 1.155, 1.144, 1.138, 1.132, 1.144, 1.127, 1.100, 1.144, 1.168]

plt.figure()
plt.plot(years_trade, coverage_values, marker='o')
plt.title("Покриття імпорту експортом (рази)")
plt.xlabel("Рік")
plt.ylabel("Коефіцієнт покриття")
plt.grid(True)
plt.savefig("export_import_ratio.png", bbox_inches="tight")
plt.close()
