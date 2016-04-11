function  [new_prices] = tax_algorithm(cur_prices, purchases)

%best_prices = cur_prices
price_change=[0,0.01, 0.02, -0.01, -0.02 ];
best_percentage = 0;
count = 0;
percs = zeros((size(price_change,2))^12,1);
tic 
for product1= price_change;
    for product2= price_change;
        for product3= price_change;
            for product4= price_change;
                for product5= price_change;
                    
                    for product6= price_change;
                        for product7= price_change;
                            
                            for product8= price_change;
                                for product9= price_change;
                                    for product10= price_change;
                                        
                                        for product11= price_change;
                                           
                                            for product12= price_change;
                                                count = count +1 ;
                                                delta_prices = [product1 product2 product3 product4 product5 product6 product7 product8 product9 product10 product11 product12];
                                                price_to_try = cur_prices + delta_prices';
                                                new_purchases = 1.13*(purchases * price_to_try);
                                                perc_round_new = sum(mod(round(100*new_purchases), 5)==0) / size(purchases,1);
                                                percs(count)= perc_round_new;
                                                if perc_round_new > best_percentage;
                                                    best_prices = price_to_try;
                                                    best_percentage = perc_round_new;
                                                end
                                            end
                                            
                                        end
                                    end
                                end
                                
                            end
                        end
                        
                    end
                    
                end
            end
        end
    end
end
toc
fprintf('best percentage is %f\n',best_percentage)
fprintf('count %d\n',count)
hist(percs)
new_prices = best_prices;
        
