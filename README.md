# Country-Methods-OOP

def test_area_valid_values():
    assert round(canada.area(unit='km2')) == 9984670
    assert round(canada.area()) == 9984670
    assert round(canada.area(unit='mi2')) == 3855081
    assert round(canada.area(unit='acres')) == 2466213490
    assert round(canada.area(unit='hectares')) == 998467000
