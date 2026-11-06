# Amsterdam Airbnb explorer (Streamlit)

A small Streamlit app that shows Airbnb listings in Amsterdam on an interactive map, next to a chosen place to visit, so you can see which affordable listings are close to it.

Built as the week 1 project ("Data and visualization") of an online course.

## What it does

- Loads about 6,000 Amsterdam listings from [`WK1_Airbnb_Amsterdam_listings_proj_solution.csv`](WK1_Airbnb_Amsterdam_listings_proj_solution.csv): listing ID, price per night, latitude, longitude, distance in meters from the chosen location, and a flag for the chosen location itself
- Keeps only listings at £100 per night or less
- Shows the filtered table
- Plots every listing and the chosen location on a Plotly map; hovering a point shows its price and distance

## Stack

Python · pandas · Plotly Express · Streamlit

## Run it locally

```bash
pip install -r requirements.txt
streamlit run streamlit_app.py
```

Streamlit opens the app in your browser at http://localhost:8501.

## Limitations and next steps

- The map uses the `stamen-terrain` style, which Plotly no longer serves; switching to `open-street-map` makes the map render again.
- The price limit is fixed in the code; a sidebar slider for budget and distance would make it a real explorer.
- Next step: deploy it on Streamlit Community Cloud and add a screenshot here.

## Author

Ami Samyra Ouedraogo · [GitHub](https://github.com/amisamyra99) · [LinkedIn](https://www.linkedin.com/in/ouedraogo-ami-samyra/)
