# Country-Methods-OOP


    assert round(usa.area(unit='km2')) == 9833520
    assert round(usa.area()) == 9833520
    assert round(usa.area(unit='mi2')) == 3796722
    assert round(usa.area(unit='acres')) == 2428879440
    assert round(usa.area(unit='hectares')) == 983352000

    assert round(canada.area(unit='km2')) == 9984670
    assert round(canada.area()) == 9984670
    assert round(canada.area(unit='mi2')) == 3855081
    assert round(canada.area(unit='acres')) == 2466213490
    assert round(canada.area(unit='hectares')) == 998467000

    assert round(usa.population_density(), 2) == 33.12
    assert round(canada.population_density(), 2) == 3.52

    assert round(usa.gdp_per_capita()) == 62014
    assert round(canada.gdp_per_capita()) == 52231

    with pytest.raises(InvalidAreaUnitException):
        usa.area(unit='INVALID')
