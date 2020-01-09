Starting this finance tracker app here!!!! JeremyG

-completed on 2016-01-21 - Had an ongoing issue with the user stocks 
not wanting to be deleted from my_portfolio page. Ended up figuring it
out removing destroy from the before_action within UserStocksController 
and adding this:
@user_stock = current_user.user_stocks.where(stock_id: params[:id]).first
to the def destroy within user_stocks_controller.rb

Rolled through this on 01/08/2020 to update and test.
